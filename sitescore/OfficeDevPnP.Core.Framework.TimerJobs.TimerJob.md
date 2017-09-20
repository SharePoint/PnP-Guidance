# TimerJob Class
 Abstract base class for creating timer jobs (background processes) that operate against SharePoint sites. These timer jobs are designed to use the CSOM API and thus can run on any server that can communicate with SharePoint.   

**Namespace:** [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public abstract class TimerJob
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [TimerJob(String)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.ctor1.md) | Simpliefied constructor for timer job, version is always set to "1.0" 
| [TimerJob(String, String)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.ctor2.md) | Simpliefied constructor for timer job, sets given version to timer job 
| [TimerJob(String, String, String)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.ctor3.md) | Default constructor for timer job 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [AuthenticationType](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.AuthenticationType.md) | Gets the authentication type that the timer job will use. This will be set as part of the UseOffice365Authentication and UseNetworkCredentialsAuthentication methods
| [ConfigurationData](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.ConfigurationData.md) | Gets or sets additional timer job configuration data
| [ExpandSubSites](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.ExpandSubSites.md) | Does the timerjob need to fire as well for every sub site in the site?
| [IsRunning](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.IsRunning.md) | Is this timer job running?
| [ManageState](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.ManageState.md) | Gets and sets the state management value: when true the timer job will automatically handle state by storing a json serialized class as a web property bag entry. Default value is false
| [MaximumThreads](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.MaximumThreads.md) | How many threads can be used by this timer job. Default value is 5.
| [Name](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.Name.md) | Gets the name of this timer job
| [Realm](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.Realm.md) | Realm will be automatically defined, but there's an option to manually specify it which may be needed when did an override of ResolveAddedSites and specify your sites.
| [SharePointVersion](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.SharePointVersion.md) | Gets or sets the SharePoint version. Default value is detected based on the laoded CSOM assembly version, but can be overriden in case you want to for example use v16 assemblies in v15 (on-premises)
| [TenantAdminSite](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.TenantAdminSite.md) | Option to specify the tenant admin site. For MT this typically is not needed since we can detect the tenant admin site, but for on premises and DvNext this is needed
| [UseThreading](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.UseThreading.md) | Can this timer job use multiple threads. Defaults to true
| [Version](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.Version.md) | Gets the version of this timer job
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [add_TimerJobRun(TimerJobRunHandler)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.fd4ee791.md) | 
| [AddSite(String)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.c9f16b09.md) | Adds a site Url or wildcard site Url to the collection of sites that the timer job will process
| [ClearAddedSites()](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.4f33069d.md) | Clears the list of added site Url's and/or wildcard site Url's
| [Clone(TimerJob)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.660f2217.md) | Takes over the settings from the passed timer job. Is useful when you run multiple jobs in a row or chain job execution. Settings that are taken over are all the authentication, enumeration settings and SharePointVersion
| [GetAllSubSites(Site)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.6810e1df.md) | Gets all sub sites for a given site
| [remove_TimerJobRun(TimerJobRunHandler)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.c2eaf49.md) | 
| [ResolveAddedSites(List&lt;String&gt;)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.f0d1233.md) | Virtual method that can be overriden to control the list of resolved sites
| [Run()](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.f2c99142.md) | Triggers the timer job to start running
| [SetEnumerationCredentials(String, String)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.99ea514b.md) | Provides the timer job with the enumeration credentials. For Office 365 username and password is sufficient
| [SetEnumerationCredentials(String, SecureString)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.a5806529.md) | Provides the timer job with the enumeration credentials. For Office 365 username and password is sufficient
| [SetEnumerationCredentials(String, String, String)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.58034b34.md) | Provides the timer job with the enumeration credentials. For SharePoint on-premises username, password and domain are needed
| [SetEnumerationCredentials(String, SecureString, String)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.e62aec94.md) | Provides the timer job with the enumeration credentials. For SharePoint on-premises username, password and domain are needed
| [SetEnumerationCredentials(String)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.b1b2b33a.md) | Provides the timer job with the enumeration credentials. For SharePoint on-premises username, password and domain are needed
| [UpdateAddedSites(List&lt;String&gt;)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.1ad1d570.md) | Virtual method that can be overriden to allow the timer job itself to control the list of sites to operate against. Scenario is for example timer job that reads this data from a database instead of being fed by the calling program
| [UseAppOnlyAuthentication(String, String)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.913e50eb.md) | Prepares the timerjob to operate against SharePoint on-premises with app-only credentials. Sets AuthenticationType to AuthenticationType.AppOnly
| [UseAzureADAppOnlyAuthentication(String, String, String, String)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.9437a92d.md) | Prepares the timerjob to operate against SharePoint Only with Azure AD app-only credentials. Sets AuthenticationType to AuthenticationType.AzureADAppOnly
| [UseAzureADAppOnlyAuthentication(String, String, String, SecureString)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.e55b0812.md) | Prepares the timerjob to operate against SharePoint Only with Azure AD app-only credentials. Sets AuthenticationType to AuthenticationType.AzureADAppOnly
| [UseAzureADAppOnlyAuthentication(String, String, X509Certificate2)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.d6643e5d.md) | Prepares the timerjob to operate against SharePoint Only with Azure AD app-only credentials. Sets AuthenticationType to AuthenticationType.AzureADAppOnly
| [UseNetworkCredentialsAuthentication(String, String, String)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.bcf4e9f6.md) | Prepares the timerjob to operate against SharePoint on-premises with user name password credentials. Sets AuthenticationType to AuthenticationType.NetworkCredentials
| [UseNetworkCredentialsAuthentication(String, SecureString, String)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.66b99329.md) | Prepares the timerjob to operate against SharePoint on-premises with user name password credentials. Sets AuthenticationType to AuthenticationType.NetworkCredentials
| [UseNetworkCredentialsAuthentication(String)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.413fa6c7.md) | Prepares the timerjob to operate against SharePoint on-premises with user name password credentials which are retrieved via the windows Credential Manager. Sets AuthenticationType to AuthenticationType.NetworkCredentials
| [UseOffice365Authentication(String, String)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.5642ea13.md) | Prepares the timerjob to operate against Office 365 with user and password credentials. Sets AuthenticationType to AuthenticationType.Office365
| [UseOffice365Authentication(String, SecureString)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.a0893d75.md) | Prepares the timerjob to operate against Office 365 with user and password credentials. Sets AuthenticationType to AuthenticationType.Office365
| [UseOffice365Authentication(String)](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.aa62ec03.md) | Prepares the timerjob to operate against Office 365 with user and password credentials which are retrieved via the windows Credential Manager. Also sets AuthenticationType to AuthenticationType.Office365
## See also
- [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md)
