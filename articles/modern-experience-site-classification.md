# SharePoint "modern" sites classification
When you create "modern" sites in SharePoint Online, you can optionally select a 'Site Classification' to define the sensitivity of your site data. The goal of site classification is to allow managing clusters of sites based on their classification from a governance and compliance perspective, as well as to automate governance processes based on site classification.

>**Important:** 
The 'Site Classification' option is not enabled by default, and you need to configure it at the Azure AD level.

_**Applies to:** SharePoint Online_

## Enabling 'Site Classification' in your tenant
<a name="enablingSiteClassification"> </a>
In order to benefit of 'Site Classification' you need to enable this capability at the Azure AD level, in your target tenant. Once you have enabled this capability, you will see an additional field 'How sensititive is your data?' while creating new "modern" sites. In the following figure you can see how the 'Site Classification' field looks like.

![The 'Site Classification' option while creating a "modern" site in SharePoint Online](media/modern-experiences/site-classification-ui.png)

While in the following figure, you can see the classification highlighted in the header of a "modern" site.

![The 'Site Classification' highlighted in the header of a "modern" site](media/modern-experiences/site-classification-ui-output.png)

To enable the capability you need to execute a bunch of PowerShell code, like the one illustrated below.

```PowerShell
# Install the AzureAD Preview Module for PowerShell
Install-Module AzureADPreview

# Connect to Azure AD
Connect-AzureAD

# Create new directory setting and set initial values
$template = Get-AzureADDirectorySettingTemplate | where { $_.DisplayName -eq "Group.Unified" }

$setting = $template.CreateDirectorySetting()
$setting["UsageGuidelinesUrl"] = "https://aka.ms/sppnp"
$setting["ClassificationList"] = "HBI, MBI, LBI, GDPR"
$setting["DefaultClassification"] = "MBI"
New-AzureADDirectorySetting -DirectorySetting $setting

```

>**Note:** 
Please, consider that it takes a while (about 1 hour or more) to have the settings available in the UI of Office 365.

About the code snippet above, it worth it to say that at the time of this writing you have to use the preview version of the AzureAD cmdlets, but pretty soon you will be able to use the RTM version.
Once you have installed the AzureAD cmdlets, you simply need to connect to the target Azure AD tenant, which is backing your target SharePoint Online tenant.
Using the _Get-AzureADDirectorySettingTemplate_ cmdlet you get a reference to the 'Setting Template' for the 'Unified Groups', which is the one with _DisplayName_ of 'Group.Unified'.
Once you have the template, you can configure the settings of that template by creating a new _DirectorySetting_ and providing the setting values through a dictionary.

The main settings, from a 'Site Classification' perspective are:
* **UsageGuidelinesUrl**: the URL of a page where you can explain what are the different classification options. A link to that page will show up in the site creation form and in the header of every classified site.
* **ClassificationList**: a comma separated list of values for the 'Site Classification' options list.
* **DefaultClassification**: the default value for the 'Site Classification'.

## Updating or Removing 'Site Classification' in your tenant
<a name="updatingRemovingClassification"> </a>
If you need to update the 'Site Classification' settings afterwards, you can use the following PowerShell snippet.

```PowerShell
# Connect to Azure AD
Connect-AzureAD

# Read current settings
(Get-AzureADDirectorySetting | where { $_.DisplayName -eq "Group.Unified" }).Values

# Update settings
$currentSettings = Get-AzureADDirectorySetting | where { $_.DisplayName -eq "Group.Unified" }
$currentSettings["UsageGuidelinesUrl"] = "https://aka.ms/sppnp"
$currentSettings["ClassificationList"] = "HBI, MBI, LBI, GDPR"
$currentSettings["DefaultClassification"] = "MBI"
Set-AzureADDirectorySetting -Id $currentSettings.Id -DirectorySetting $currentSettings

```

>**Note:** 
Please, consider that it takes a while (about 1 hour or more) to have the settings updated in the UI of Office 365. However, it shouldn't be a big issue, because you shouldn't update the 'Site Classification' settings very often.

As you can see, you simply need to search for the Directory Setting with a _DisplayName_ value of 'Group.Unified' and then you can update its setting values and apply the changes by using the _Set-AzureADDirectorySetting_ cmdlet.

To remove a 'Site Classification' you can use the _Remove-AzureADDirectorySetting_ cmdlet, like in the following code snippet.

```PowerShell
# Delete settings
$currentSettings = Get-AzureADDirectorySetting | where { $_.DisplayName -eq "Group.Unified" }
Remove-AzureADDirectorySetting -Id $currentSettings.Id
```

## Managing the classification of a site
<a name="managingClassification"> </a>
The value of classification for a site can be read, or updated, later on using the UI of SharePoint Online, as you can see in the following figure, by editing the 'Site Information' settings.

![The 'Site Classification' option while editing the 'Site Information' settings of a "modern" site in SharePoint Online](media/modern-experiences/site-classification-update-ui.png)

### Programmatically reading the classification of a site
<a name="sectionSection3"> </a>
From a developer's perspective, you can also use CSOM and the REST API of SharePoint Online. In fact, every SharePoint Online site collection has the _Classification_ property that you can use to read the site classification. Here you can see a PowerShell snippet to do that.

```PowerShell
# Delete settings
Connect-PnPOnline "https://[tenant].sharepoint.com/sites/[modernsite]" -Credentials [credentials]

$site = Get-PnPSite
$classificationValue = Get-PnPProperty -ClientObject $site -Property Classification
Write-Host $classificationValue
```

If you like to read the 'Site Classification' value using REST, for example within a SharePoint Framework client-side web part, you can use the following REST endpoint:

```TEXT
https://[tenant].sharepoint.com/sites/[modernsite]/_api/site/Classification
```

Based on the classification value of a site, you can define automation and custom policy rules.

### Programmatically updating the classification of a site
<a name="governanceClassification"> </a>
If your target is a  "modern" communication site, you can use the _Classification_ property of CSOM to update the value, too.

If your target is a "modern" team site and you want to update the classification value, you should use the Microsoft Graph because the _Classification_ property of CSOM simply replicates the value of the _classification_ property of the Office 365 Group.

> **Note**: You can find further details about how to update an Office 365 Group using the Microsoft Graph in the document [Update group](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/group_update).
