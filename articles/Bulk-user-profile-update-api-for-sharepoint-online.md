# Introducing the API for bulk custom user profile properties update for SharePoint Online


_**Applies to:** SharePoint Online_

As part of the new Client Side Object Model (CSOM) version (4622.1208 or newer), SharePoint has new capability for bulk importing custom user profile properties. Previously you could have taken advantage of the user profile CSOM operations for updating specific properties for user profiles, but this is not that performant and in case of thousands of profiles, the operation is too time consuming.

Since many enterprises however have business requirements to replicate custom attributes to the SharePoint user profile service a more performant user profile bulk API has been released.

## Bulk user profile update flow
<a name="sectionSection0"> </a>

![Bulk UPA update flow](media/bulkuserprofileupdateapi/UserProfileBulkAPIProcess.png)

1. User attributes are synchronized from the corporate Active Directory to the Azure Active Directory. You can select which attributes are being replicated cross on-premises and Azure
2. Standardized set of attributes are being replicated from the Azure Active Directory to SharePoint user profile store at Office 365. This cannot be controlled like in the on-premises.
3. A custom synchronization tool taking advantage of the new build update APIs. This tool uploads a JSON formatted file to Office 365 tenant and queues the import process. Implemented as managed code (.NET) or as PowerShell script using the new CSOM APIs.
4. LOB system or any external system, which is the actual source of the information in the JSON formatted file. This could be also combination of data from Active Directory and from any external system. Notice that from an API perspective, the LOB system could be also on-premises SharePoint 2013 or 2016 deployment from where you’d synchronize user profile attributes to SharePoint online.
5. Out of the box server side timer job running in SharePoint online, which checks for queued import requests and will perform the actual import operation based on the API calls and information in provided file.
6. Extended user profile information is available in the user profile and can be used for any out of the box or custom functionality in the SharePoint online.

>**Note**: Import only works for user profile properties, which has not been set to be editable for the end users. This is to avoid situation where the user profile import process would override any information which end user has already updated. Also import only allows custom properties that are not active directory core properties that typically must be synchronized to Azure Active Directory. For list of typical core directory properties see table listed later in FAQ section at this blog post.

Here's quick demo video on using the new CSOM API from managed code or from PowerShell. You can find used code sample, including sample PowerShell script, from the [Office Dev PnP Code Gallery](http://dev.office.com/patterns-and-practices-detail/7202).

<iframe id="ytplayer" type="text/html" width="640" height="390" src="https://www.youtube.com/embed/-X_2T0SRUBk?autoplay=0&origin=https://msdn.microsoft.com" frameborder="0"></iframe>

## Import file format
<a name="sectionSection1"> </a>

Information to be processed is provided with JSON formatted file. Here’s a structure for the file format.   

```JSON
{
   "value": [
     {
       "<IdName>": "<UserIdValue_1>",
       "<AttributeName_1>": "<User1_AttributedValue_1>",
       "<AttributeName_2>": "<User1_AttributedValue_2>",
     },
     {
       "<IdName>": "<UserIdValue_2>",
       "<AttributeName_1>": "<User2_AttributedValue_1>",
       "<AttributeName_2>": "<User2_AttributedValue_2>",
     },
     {
       "<IdName>": "<UserIdValue_n>",
       "<AttributeName_1>": "<Usern_AttributedValue_1>",
       "<AttributeName_2>": "<Usern_AttributedValue_2>",
     }
   ]
}
```

Here’s simple example file. Identity resolution in this case will be based on the `IdName` property and we have three different properties, which are being updated called `City` and `Office`. File contains information for four different accounts in the specific tenant. Property names used in the source file are not locked on the names used in the SharePoint Online user profile service, since we will provide correct property mapping for the information within our code. 

```JSON
{
  "value": [
    {
      "IdName": "vesaj@contoso.com",
      "Property1": "Helsinki",
      "Property2": "Viper"
    },
    {
      "IdName": "bjansen@contoso.com",
      "Property1": "Brussels",
      "Property2": "Beetle"
    },
    {
      "IdName": "unknowperson@contoso.com",
      "Property1": "None",
      "Property2": ""
    },
    {
      "IdName": "erwin@contoso.com",
      "Property1": "Stockholm",
      "Property2": "Elite"
    }
  ]
}
```

### Source data restrictions
There are few restrictions on the source data as presented here:
- Max size: 2GB
- Max properties: 500,000
- Source file must be uploaded to same SharePoint Online tenant where the process is started


## User profile property import process
<a name="sectionSection2"> </a>

Here’s the full process:

1. Create or synchronize users to Office 365 tenant or to Azure AD associated to it
	 - When users are synchronized to Azure AD, it will also synchronize standardized set of attributes to SharePoint online User Profile Service.
2. Create needed custom properties in the User Profile Service
	 - Since there’s no remote APIs for creating custom properties to User Profile Service this step has to be performed manually once for each of the tenants where custom user profile properties are needed.
	 - Notice that only user profile properties which are not “allowed to be edit by end users” can be imported. Trying to import JSON object property to a user profile property, which is marked as “editable by end users” will result an exception when CSOM API is called.
3. Create and upload external data file to Office 365 tenant
	 - You’ll need to upload the JSON formatted data file containing the information to be updated to the particular Office 365 tenant.
	 - Notice that in case of any exception during actual import process, SharePoint will provide additional logging information which is saved automatically to the same document library where the file existed with a new sub folder.
	 - Cleaning of the log files and provided JSON files are on the responsibility of the custom solution using the API. You should consider the life cycle of these files in your implementation. Files are stored in the document libraries, so they will be consuming assigned storage for the site collection.
4. Call bulk UPA Import API for queuing the import job
	 - Use the CSOM API to queue up the import process. This can be achieved by executing CSOM code by using managed code or PowerShell.
	 - Method call to queue up the job will require property mapping information and the location of the data file. This method execution will be fast and it will just queue up the actual import process, which will be executed as back end process in the SharePoint Online.
5. Check status of the import job
	 - You can also use remote APIs to check the status of specific import job or for all of the import jobs done recently. To be able to check status of specific call, you should store the unique job identifier which is received as return value when the job is queued up.


## CSOM API for bulk import process
<a name="sectionSection3"> </a>

### Queue import
You can queue import process by calling QueueImportProfileProperties method located in the Office365Tenant object. This is asynchronous call in a way that it doesn’t download the source data or the import, it simply adds work item to queue for doing this later. Here’s the full signature of the method:

```c#
public ClientResult<Guid> QueueImportProfileProperties(
                          ImportProfilePropertiesUserIdType idType, 
                          string sourceDataIdProperty, 
                          IDictionary<string, string> propertyMap, 
                          string sourceUri);
```

#### Parameters

**idType**
*Type: ImportProfilePropertiesUserIdType*

The type of id to use when looking up the user profile. Possible values are Email, CloudId and PrincipalName. Referring on how to resolve the identity at the cloud, either using email, Azure AD id or principal name. Note that regardless of the type the user must already exist in the User Profile Service for import to work. It’s recommended to use the Cloud SID is the option to resolve the identifying property to ensure uniqueness.

Property mapping between ID Type and Azure AD property:
- UPA Bulk Import ID Type 
- Azure Directory Attribute
- CloudSID
- ObjectID
- PrincipalName
- userPrincipalName
- Email
- mail

**sourceDataIdProperty**
*Type: System.String*

The name of the id property in the source data. The value of the property from the source data will be used to look up the user. The User Profile Service property used for the lookup depends on the value of idType.

**propertyMap**
*Type: IDictionary<string, string>*

A map from source property name to User Profile Service property name. Note that the User Profile Service properties must already exist.

**sourceUri**
*Type: System.String*

The URI of the source data to import. This must not be transient as it may not be downloaded for some time.

#### Return value
Guid identifying the import job that has been queued.
Here's a sample code to start the process with sample input file.

```c#
// Create instance to Office 365 Tenant object. Technically not needed to load though. 
Office365Tenant tenant = new Office365Tenant(ctx);
ctx.Load(tenant);
ctx.ExecuteQuery();

// Type of user identifier ["PrincipleName", "EmailAddress", "CloudId"] in the 
// User Profile Service. In this case we use email as the identifier at the UPA storage
ImportProfilePropertiesUserIdType userIdType = 
      ImportProfilePropertiesUserIdType.Email;

// Name of user identifier property in the JSON file
var userLookupKey = "IdName";

var propertyMap = new System.Collections.Generic.Dictionary<string, string>();

// First one is the property at the JSON file, 
// second is the user profile property Name at User Profile Service
// Notice that we have here 2 custom properties in UPA called 'City' and 'OfficeCode'
propertyMap.Add("City", "City");
propertyMap.Add("Office", "OfficeCode");

// Returns a GUID, which can be used to see the status of the execution and end results
var workItemId = tenant.QueueImportProfileProperties(
      userIdType, userLookupKey, propertyMap, fileUrl
      );

ctx.ExecuteQuery();
```

### Check status of import job
You can also check status of the User Profile Service import jobs by using new CSOM APIs. There’s two new methods for this in the Tenant object.
You can check status of individual import job by using GetImportProfilePropertyJob method located in the Office365Tenant object. You will need to have the unique identifier of specific import job provided as a parameter for this method. Here’s the full signature of the method:

```c#
public ImportProfilePropertiesJobInfo GetImportProfilePropertyJob(Guid jobId);
```

#### Parameters
**jobID**
*Type: Guid*

The id of the job for which to get high-level status.

#### Return value

An `ImportProfilePropertiesJobStatus` object with high level status information about the specified job.

Here’s a sample code to get status of specific import job using stored identifier.

```c#
// Check status of specific request based on job id received when we queued the job
Office365Tenant tenant = new Office365Tenant(ctx);
var job = tenant.GetImportProfilePropertyJob(workItemId);
ctx.Load(job);
ctx.ExecuteQuery();
```

You can check status of all import jobs by using GetImportProfilePropertyJobs method located in the Office365Tenant object. Here’s the full signature of the method:

```c#
public ImportProfilePropertiesJobStatusCollection GetImportProfilePropertyJobs(); 
```

Return value
An `ImportProfilePropertiesJobStatusCollection` object which is collection of ImportProfilePropertiesJobStatus objects with high level status information about the specified jobs.

Here’s a sample code to get status of all import jobs currently saved in the tenant. These could be already processed or queued jobs.

```c#
// Load all import jobs – old and queued ones
Office365Tenant tenant = new Office365Tenant(ctx);
var jobs = tenant.GetImportProfilePropertyJobs();
ctx.Load(jobs);
ctx.ExecuteQuery();
foreach (var item in jobs)
{
   // Check whatever properties needed
   var state = item.State;
}
```

`ImportProfilePropertiesJobStatus` object returned with the import status information has following properties. 

**JobId** - *Guid*
The Id of the import job

**State** - *ImportProfilePropertiesJobState*
An enum that has the following values:
- Unknown We cannot determine the state of the job
- Submitted The job has been submitted to the system
- Processing The job is being processed
- Queued The job has passed validation and queued for import to UPA
- Succeeded The job completed with no error
- Error The job completed with error

**SourceUri** - *Uri*
The URI to the data source file

**Error** - *ImportProfilePropertiesJobError*
An enum representing the possible error:
- NoError No error found
- InternalError The error caused by a failure in the service
- DataFileNotExist The data source file cannot be found
- DataFileNotInTenant The data source file does not belong to the same tenant
- DataFileTooBig The size of the data file is too big
- InvalideDataFile The data source file does not pass the validation. There might be more detailes in the log file
- ImportCompelteWithErrors The data has been imported, but there is some error encountered

**ErrorMessage** *String*
The eror message

**LogFileUri** - *Uri*
The Uri to the folder where the logs have been written

## Calling Import API from PowerShell
<a name="sectionSection4"> </a>

You can take advantage of the User Profile Service bulk import API with PowerShell. This means that you’ll use the CSOM code directly in the PowerShell script with the needed parameters. This requires that the updated CSOM redistributable package has been installed on the used computer where the script is executed.
By using PowerShell, you do not need to specifically combine your code within Visual Studio, which could be more suitable model for some customers depending on the exact business scenarios.

### Sample script
Here’s a sample PowerShell script which performs the same operation as the code previously in this document. 

```Powershell
# Get needed information from end user
$adminUrl = Read-Host -Prompt 'Enter the admin URL of your tenant'
$userName = Read-Host -Prompt 'Enter your user name'
$pwd = Read-Host -Prompt 'Enter your password' -AsSecureString
$importFileUrl = Read-Host -Prompt 'Enter the URL to the file located in your tenant'

# Get instances to the Office 365 tenant using CSOM
$uri = New-Object System.Uri -ArgumentList $adminUrl
$context = New-Object Microsoft.SharePoint.Client.ClientContext($uri)

$context.Credentials = New-Object Microsoft.SharePoint.Client.SharePointOnlineCredentials($userName, $pwd)
$o365 = New-Object Microsoft.Online.SharePoint.TenantManagement.Office365Tenant($context)
$context.Load($o365)

# Type of user identifier ["Email", "CloudId", "PrincipalName"] in the User Profile Service
$userIdType=[Microsoft.Online.SharePoint.TenantManagement.ImportProfilePropertiesUserIdType]::Email

# Name of user identifier property in the JSON
$userLookupKey="idName"

# Create property mapping between on-premises name and O365 property name
# Notice that we have here 2 custom properties in UPA called 'City' and 'OfficeCode'
$propertyMap = New-Object -type 'System.Collections.Generic.Dictionary[String,String]'
$propertyMap.Add("Property1", "City")
$propertyMap.Add("Property2", "OfficeCode")

# Call to queue UPA property import 
$workItemId = $o365.QueueImportProfileProperties($userIdType, $userLookupKey, $propertyMap, $importFileUrl);

# Execute the CSOM command for queuing the import job
$context.ExecuteQuery();

# Output unique identifier of the job
Write-Host "Import job created with following identifier:" $workItemId.Value 
```

## Exception process
<a name="sectionSection5"> </a>
There’s two level of checking of the provided information when this API is used. When you queue up the import process with the CSOM, there will be initial level of checking on the provided values, like confirmation that the provided mapping properties exists in the User Profile Service and that property is not editable by the end user. When queue API is called, only initial level of verification is applied and final verification of the provided information is performed when the import job is actually executed.

If there’s any exceptions during the actual import job execution, additional logging file with needed details is generated to same document library where the import file was located. Log files for specific import job are being saved to sub folders named using the unique identifier of the specific import job.

Here’s an example result from one import in the document library where the import file was located. In the below picture you can see two sub folders for two different executions created on the document library where the import file is stored.

![Exception process](media/bulkuserprofileupdateapi/UserProfileBulkAPIProcess-folders.png)

Actual log file is saved in the sub folder and you can download that from the Office 365 for detailed analyses. 

![Exception process](media/bulkuserprofileupdateapi/UserProfileBulkAPIProcess-LogFile.png)

### Common exceptions and description

Following table contains typical exceptions which you could encounter when you start using the User Profile Service bulk API.

**Exception**: *Property Names [AboutMe] are editable by user.*
This would be thrown by the CSOM API when you call ExecuteQuery method for submitting the job to your tenant. API will check that all properties currently being mapped for the property mapping are NOT user editable. Exception will point out the property which is cannot be used. In this example case we have tried to map a JSON property to AboutMe property in the User Profile Service properties, but this is not allowed, since AboutMe is user editable property.

**Exception**: *InvalidProperty - vesaj@contoso.com Property 'AboutMe' is not mapped to any property in the user profile application.*
JSON data file contained a property which has not been mapped to the User Profile Service property in SharePoint Online. This means that source data file is containing properties, which you have not assigned proper mapping. You will need to have mapping definition provided for the QueueImportProfileProperties method for each of the properties in the JSON data object.

**Exception**: *MissingIdentity - The identity is missing for the user object*
Identity property could not be found from the user object. Most likely cause is that the sourceDataIdProperty attribute is wrongly set for the QueueImportProfileProperties method.Ensure that you have right property in the JSON source file and that your code/script is assigning this attribute accordingly based on the data file content.

**Exception**: *IdentityNotResolvable unknown@contoso.com User identity cannot be resolved*
Data file contained an identity, which could not be resolved or was not present in the User Profile Service. In this case the user profile with email of unknown@contoso.com could not be located in the User Profile Service.

**Exception**: *DataFileNotJson - JsonToken EndObject is not valid for closing JsonType Array. Path 'value', line 8, position 10.*
Your import file format is not valid JSON and does not match the excepted format. 

## Questions and answers
<a name="sectionSection6"> </a>

**Can I execute the code using app-only/add-in only permissions?**
Yes – this is absolutely possible. You’ll need to register client id and secret to be able to execute the APIs. Since actual import of the file does not occur synchronously with the identity of the caller, this works without any issues.

**This API is updating properties in the User Profile Service, but how would I create those properties in the tenant?**
There’s no remote API to create custom user profile properties programmatically, so this is manual operation which needs to be completed once per given tenant. You can refer to this article for instructions on how to create these custom properties.

**Is this capability available in the on-premises SharePoint?**
This capability is unfortunately only for SharePoint Online at least for now. In on-premises SharePoint this capability would be useful but not as much needed, since you can modify attribute mapping in the on-premises user profile service application. You could also take advantage of importing user profile attributes using Business Continuity Service (BCS) in SharePoint 2013, but this option is not available in SP2016, which means that in the case of SP2016 you only option currenly is to implement customizations which take advantage of the user profile web services.

**Could I use this API for synchronizing user profile property values from my on-premises SharePoint 2013 or 2016 to SharePoint Online?**
Yes. On-premises SharePoint would be considered as any source system. You’d have to export the user profile values from your on-premises SharePoint to JSON file format and process would be exactly the same as importing values from any other system.

**Can I import string based multi-value properties?**
No. This is not currently supported with this API.

**What permissions are required for executing this API??**
You will need to have Global Admin permissions currently. SharePoint Admin is not sufficient.

**Can I import taxonomy based multi-value properties?**
No. This is not currently supported with this API.

**What if I define mapping in the code which is not used or have property in the JSON which is not mapped?**
If your code/script defines a mapping which is not used or data file does not contain properties for that mapping, execution will continue without any exceptions and import will be applied based on mapped properties. If you however have property in the JSON file which is not mapped, import process will be aborted and exception details will be provided in the log file for the specific job execution.

**What if I have a need to update custom properties that are beyond the size limitations of this bulk API (i.e. >2 GB file or >500,000 properties)?**
You would need to batch your jobs accordingly by triggering multiple jobs in sequence i.e. finishing one job at a time with the maximum limit on this API. You should expect these high bandwidth imports will take a long time to complete. Also, you should optimize the import jobs only for delta changes in custom profile properties rather than importing full set of values in all jobs.

**Which Azure Active Directory attributes are being sync’d to SharePoint Online user profile by default?**
See following table for the official list of synchronized attributes and their mapping between Azure Active Directory and SharePoint Online User Profile.

Azure Directory Attribute  | SharePoint Online Profile Property
---------|----------
ObjectSid | SPS-SavedSID
msonline-UserPrincipalName | UserName
msonline-UserPrincipalName | AccountName
msonline-UserPrincipalName | SPS-ClaimID
msonline-UserPrincipalName | SPS-UserPrincipalName
GivenName | FirstName
sn | LastName
Manager | Manager
DisplayName | PreferredName
telephoneNumber | WorkPhone
proxyAddresses | WorkEmail
proxyAddresses | SPS-SIPAddress
PhysicalDeliveryOfficeName | Office
Title | Title
Title | SPS-JobTitle
Department | Department
Department | SPS-Department
ObjectGuid | ADGuid
WWWHomePage | PublicSiteRedirect
DistinguishedName | SPS-DistinguishedName
msOnline-ObjectId | msOnline-ObjectId
PreferredLanguage | SPS-MUILanguages
msExchHideFromAddressList | SPS-HideFromAddressLists
msExchRecipientTypeDetails | SPS-RecipientTypeDetails
msonline-groupType | IsUnifiedGroup
msOnline-IsPublic | IsPublic
msOnline-ObjectId | msOnline-ObjectId
msOnline-UserType | SPS-UserType
GroupType | GroupType
SPO-IsSharePointOnlineObject | SPO-IsSPO

