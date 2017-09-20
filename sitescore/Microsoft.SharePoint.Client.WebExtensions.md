# WebExtensions Class
 Class that holds deprecated methods for site (both site collection and web site) creation, status, retrieval and settings 

 Class that deals with site (both site collection and web site) creation, status, retrieval and settings   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class WebExtensions
```
## Extension Methods
|**Name**|**Description**|
|:-----|:-----|
| [AddIndexedPropertyBagKey(Web, String)](Microsoft.SharePoint.Client.WebExtensions.1e21757a.md) | Marks a property bag key for indexing
| [AddRemoteEventReceiver(Web, String, String, EventReceiverType, EventReceiverSynchronization, Boolean)](Microsoft.SharePoint.Client.WebExtensions.e1c51dcb.md) | Registers a remote event receiver
| [AddRemoteEventReceiver(Web, String, String, EventReceiverType, EventReceiverSynchronization, Int32, Boolean)](Microsoft.SharePoint.Client.WebExtensions.4c2af14e.md) | Registers a remote event receiver
| [ApplyProvisioningTemplate(Web, ProvisioningTemplate, ProvisioningTemplateApplyingInformation)](Microsoft.SharePoint.Client.WebExtensions.5fdc38cc.md) | Can be used to apply custom remote provisioning template on top of existing site.
| [CreateWeb(Web, SiteEntity, Boolean, Boolean)](Microsoft.SharePoint.Client.WebExtensions.6792428f.md) | Adds a new child Web (site) to a parent Web.
| [CreateWeb(Web, String, String, String, String, Int32, Boolean, Boolean)](Microsoft.SharePoint.Client.WebExtensions.593e8e9d.md) | Adds a new child Web (site) to a parent Web.
| [DeleteWeb(Web, String)](Microsoft.SharePoint.Client.WebExtensions.34d305de.md) | Deletes the child website with the specified leaf URL, from a parent Web, if it exists.
| [DeployApplicationPackageToAppCatalog(Web, String, String, Boolean, Boolean)](Microsoft.SharePoint.Client.WebExtensions.a38d0e24.md) | Adds a package to the tenants app catalog and by default deploys it if the package is a client side package (sppkg)
| [DeployApplicationPackageToAppCatalog(Web, String, String, Boolean, Boolean, Boolean)](Microsoft.SharePoint.Client.WebExtensions.ac37d25e.md) | Adds a package to the tenants app catalog and by default deploys it if the package is a client side package (sppkg)
| [DisableRequestAccess(Web)](Microsoft.SharePoint.Client.WebExtensions.1fec6f8d.md) | Disables the request access on the web.
| [EnableRequestAccess(Web, String[])](Microsoft.SharePoint.Client.WebExtensions.a6aeb360.md) | Enables request access for the specified e-mail addresses.
| [EnableRequestAccess(Web, IEnumerable&lt;String&gt;)](Microsoft.SharePoint.Client.WebExtensions.efaf0293.md) | Enables request access for the specified e-mail addresses.
| [GetAllWebUrls(Site)](Microsoft.SharePoint.Client.WebExtensions.3201f18f.md) | Gets the collection of the URLs of all Web sites that are contained within the site collection, including the top-level site and its subsites.
| [GetAppCatalog(Web)](Microsoft.SharePoint.Client.WebExtensions.c6c34651.md) | Gets the Uri for the tenant's app catalog site (if that one has already been created)
| [GetAppInstances(Web, Expression&lt;Func&lt;AppInstance, Object&gt;&gt;[])](Microsoft.SharePoint.Client.WebExtensions.b057f688.md) | Returns all app instances
| [GetBaseTemplateId(Web)](Microsoft.SharePoint.Client.WebExtensions.f90c56f2.md) | Returns the Base Template ID for the current web
| [GetEventReceiverById(Web, Guid)](Microsoft.SharePoint.Client.WebExtensions.a2bbb95b.md) | Returns an event receiver definition
| [GetEventReceiverByName(Web, String)](Microsoft.SharePoint.Client.WebExtensions.f3860fda.md) | Returns an event receiver definition
| [GetIndexedPropertyBagKeys(Web)](Microsoft.SharePoint.Client.WebExtensions.fc2a9547.md) | Returns all keys in the property bag that have been marked for indexing
| [GetPropertyBagValueDateTime(Web, String, DateTime)](Microsoft.SharePoint.Client.WebExtensions.fdfebc13.md) | Get DateTime typed property bag value. If does not contain, returns default value.
| [GetPropertyBagValueInt(Web, String, Int32)](Microsoft.SharePoint.Client.WebExtensions.fb0e8960.md) | Get int typed property bag value. If does not contain, returns default value.
| [GetPropertyBagValueString(Web, String, String)](Microsoft.SharePoint.Client.WebExtensions.4427b00a.md) | Get string typed property bag value. If does not contain, returns given default value.
| [GetProvisioningTemplate(Web)](Microsoft.SharePoint.Client.WebExtensions.58235816.md) | Can be used to extract custom provisioning template from existing site. The extracted template will be compared with the default base template.
| [GetProvisioningTemplate(Web, ProvisioningTemplateCreationInformation)](Microsoft.SharePoint.Client.WebExtensions.8e22f686.md) | Can be used to extract custom provisioning template from existing site. The extracted template will be compared with the default base template.
| [GetRequestAccessEmails(Web)](Microsoft.SharePoint.Client.WebExtensions.e3474ac6.md) | Gets the request access e-mail addresses of the web.
| [GetWeb(Web, String)](Microsoft.SharePoint.Client.WebExtensions.f4d9ae5b.md) | Returns the child Web site with the specified leaf URL.
| [InstallSolution(Site, Guid, String, Int32, Int32)](Microsoft.SharePoint.Client.WebExtensions.8e60cd11.md) | Uploads and installs a sandbox solution package (.WSP) file, replacing existing solution if necessary.
| [IsNoScriptSite(Site)](Microsoft.SharePoint.Client.WebExtensions.f9298408.md) | Detects if the site in question has no script enabled or not. Detection is done by verifying if the AddAndCustomizePages permission is missing. See https://support.office.com/en-us/article/Turn-scripting-capabilities-on-or-off-1f2c515f-5d7e-448a-9fd7-835da935584f for the effects of NoScript
| [IsNoScriptSite(Web)](Microsoft.SharePoint.Client.WebExtensions.e5b2b186.md) | Detects if the site in question has no script enabled or not. Detection is done by verifying if the AddAndCustomizePages permission is missing. See https://support.office.com/en-us/article/Turn-scripting-capabilities-on-or-off-1f2c515f-5d7e-448a-9fd7-835da935584f for the effects of NoScript
| [IsPublishingWeb(Web)](Microsoft.SharePoint.Client.WebExtensions.471e4515.md) | Checks if the current web is a publishing site or not
| [IsSubSite(Web)](Microsoft.SharePoint.Client.WebExtensions.3f4614d5.md) | Checks if the current web is a sub site or not
| [MySiteSearch(Web)](Microsoft.SharePoint.Client.WebExtensions.cd9358ce.md) | Returns all my site site collections
| [PropertyBagContainsKey(Web, String)](Microsoft.SharePoint.Client.WebExtensions.7a7ae50c.md) | Checks if the given property bag entry exists
| [ReIndexWeb(Web)](Microsoft.SharePoint.Client.WebExtensions.3fc076f8.md) | Queues a web for a full crawl the next incremental/continous crawl
| [RemoveAppInstanceByTitle(Web, String)](Microsoft.SharePoint.Client.WebExtensions.ce847939.md) | Removes the app instance with the specified title.
| [RemoveIndexedPropertyBagKey(Web, String)](Microsoft.SharePoint.Client.WebExtensions.d4650ef6.md) | Unmarks a property bag key for indexing
| [RemovePropertyBagValue(Web, String)](Microsoft.SharePoint.Client.WebExtensions.7ebf8d0f.md) | Removes a property bag value from the property bag
| [SetLocalizationLabels(Web, String, String, String)](Microsoft.SharePoint.Client.WebExtensions.4fc70325.md) | Can be used to set translations for different cultures.
| [SetPageOutputCache(Web, Boolean, Int32, Int32, Boolean)](Microsoft.SharePoint.Client.WebExtensions.6f3ddc09.md) | Sets output cache on publishing web. The settings can be maintained from UI by visiting url /_layouts/15/sitecachesettings.aspx
| [SetPropertyBagValue(Web, String, Int32)](Microsoft.SharePoint.Client.WebExtensions.62c0b9da.md) | Sets a key/value pair in the web property bag
| [SetPropertyBagValue(Web, String, String)](Microsoft.SharePoint.Client.WebExtensions.e498740a.md) | Sets a key/value pair in the web property bag
| [SetPropertyBagValue(Web, String, DateTime)](Microsoft.SharePoint.Client.WebExtensions.c46c00d1.md) | Sets a key/value pair in the web property bag
| [SiteSearch(Web)](Microsoft.SharePoint.Client.WebExtensions.96462f9d.md) | Returns all site collections that are indexed. In MT the search center, mysite host and contenttype hub are defined as non indexable by default and thus are not returned
| [SiteSearch(Web, String, Boolean)](Microsoft.SharePoint.Client.WebExtensions.fdaf2ce0.md) | Returns the site collections that comply with the passed keyword query
| [SiteSearchScopedByTitle(Web, String)](Microsoft.SharePoint.Client.WebExtensions.9fff44d9.md) | Returns all site collection that match with the provided title
| [SiteSearchScopedByUrl(Web, String)](Microsoft.SharePoint.Client.WebExtensions.2aa306d6.md) | Returns all site collection that start with the provided URL
| [UninstallSolution(Site, Guid, String, Int32, Int32)](Microsoft.SharePoint.Client.WebExtensions.cb455e2d.md) | Uninstalls a sandbox solution package (.WSP) file
| [WebExists(Web, String)](Microsoft.SharePoint.Client.WebExtensions.9faba1e2.md) | Determines if a child Web site with the specified leaf URL exists.
| [WebExistsByTitle(Web, String)](Microsoft.SharePoint.Client.WebExtensions.d29a4f65.md) | Determines if a web exists by title.
| [WebExistsFullUrl(ClientRuntimeContext, String)](Microsoft.SharePoint.Client.WebExtensions.5f46fd34.md) | Determines if a Web (site) exists at the specified full URL, either accessible or that returns an access error.
## Examples
```C#
web.SetLocalizationForSiteLabels("fi-fi", "Name of the site in Finnish", "Description in Finnish");
            
```

## See also
- [http://blogs.msdn.com/b/vesku/archive/2014/03/20/office365-multilingual-content-types-site-columns-and-site-other-elements.aspx](http://blogs.msdn.com/b/vesku/archive/2014/03/20/office365-multilingual-content-types-site-columns-and-site-other-elements.aspx)
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)
