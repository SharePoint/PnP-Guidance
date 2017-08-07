# TenantExtensions Class
 Class for deprecated tenant extension methods 

 Class for tenant extension methods   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class TenantExtensions
```
## Extension Methods
|**Name**|**Description**|
|:-----|:-----|
| [AddAdministrators(Tenant, IEnumerable&lt;UserEntity&gt;, Uri, Boolean)](Microsoft.SharePoint.Client.TenantExtensions.23dcea4d.md) | Add a site collection administrator to a site collection
| [CheckIfSiteExists(Tenant, String, String)](Microsoft.SharePoint.Client.TenantExtensions.bd62d116.md) | Returns if a site collection is in a particular status. If the url contains a sub site then returns true is the sub site exists, false if not. Status is irrelevant for sub sites
| [CreateSiteCollection(Tenant, SiteEntity, Boolean, Boolean, Func&lt;TenantOperationMessage, Boolean&gt;)](Microsoft.SharePoint.Client.TenantExtensions.8f180b3b.md) | Adds a SiteEntity by launching site collection creation and waits for the creation to finish
| [CreateSiteCollection(Tenant, String, String, String, String, Int32, Int32, Int32, Int32, Int32, UInt32, Boolean, Boolean, Func&lt;TenantOperationMessage, Boolean&gt;)](Microsoft.SharePoint.Client.TenantExtensions.5122ed46.md) | Launches a site collection creation and waits for the creation to finish
| [DeleteSiteCollection(Tenant, String, Boolean, Func&lt;TenantOperationMessage, Boolean&gt;)](Microsoft.SharePoint.Client.TenantExtensions.32ab407c.md) | Deletes a site collection
| [DeleteSiteCollectionFromRecycleBin(Tenant, String, Boolean, Func&lt;TenantOperationMessage, Boolean&gt;)](Microsoft.SharePoint.Client.TenantExtensions.802142c7.md) | Deletes a site collection from the site collection recycle bin
| [DeployApplicationPackageToAppCatalog(Tenant, String, String, Boolean, Boolean)](Microsoft.SharePoint.Client.TenantExtensions.a085302b.md) | Adds a package to the tenants app catalog and by default deploys it if the package is a client side package (sppkg)
| [DeployApplicationPackageToAppCatalog(Tenant, String, String, Boolean, Boolean, Boolean)](Microsoft.SharePoint.Client.TenantExtensions.634fcfa3.md) | Adds a package to the tenants app catalog and by default deploys it if the package is a client side package (sppkg)
| [DeployApplicationPackageToAppCatalog(Tenant, String, String, String, Boolean, Boolean)](Microsoft.SharePoint.Client.TenantExtensions.8b800134.md) | Adds a package to the tenants app catalog and by default deploys it if the package is a client side package (sppkg)
| [GetAppCatalog(Tenant)](Microsoft.SharePoint.Client.TenantExtensions.a8d6a2c2.md) | Gets the Uri for the tenant's app catalog site (if that one has already been created)
| [GetOneDriveSiteCollections(Tenant)](Microsoft.SharePoint.Client.TenantExtensions.2c08e126.md) | Get OneDrive site collections by iterating through all user profiles.
| [GetSiteCollections(Tenant, Int32, Int32, Boolean, Boolean)](Microsoft.SharePoint.Client.TenantExtensions.9ce74f2.md) | Returns all site collections in the current Tenant based on a startIndex. IncludeDetail adds additional properties to the SPSite object.
| [GetSiteGuidByUrl(Tenant, String)](Microsoft.SharePoint.Client.TenantExtensions.6b408500.md) | Gets the ID of site collection with specified URL
| [GetSiteGuidByUrl(Tenant, Uri)](Microsoft.SharePoint.Client.TenantExtensions.64e4cb66.md) | Gets the ID of site collection with specified URL
| [GetUserProfileServiceClient(Tenant)](Microsoft.SharePoint.Client.TenantExtensions.4a97c99c.md) | Gets the UserProfileService proxy to enable calls to the UPA web service.
| [GetWebTemplates(Tenant, UInt32, Int32)](Microsoft.SharePoint.Client.TenantExtensions.26f04e93.md) | Returns available webtemplates/site definitions
| [IsSiteActive(Tenant, String)](Microsoft.SharePoint.Client.TenantExtensions.df897728.md) | Checks if a site collection is Active
| [SetSiteLockState(Tenant, String, SiteLockState, Boolean, Func&lt;TenantOperationMessage, Boolean&gt;)](Microsoft.SharePoint.Client.TenantExtensions.ef999b08.md) | Sets a site to Unlock access or NoAccess. This operation may occur immediately, but the site lock may take a short while before it goes into effect.
| [SetSiteProperties(Tenant, String, String, Nullable&lt;Boolean&gt;, Nullable&lt;SharingCapabilities&gt;, Nullable&lt;Int64&gt;, Nullable&lt;Int64&gt;, Nullable&lt;Double&gt;, Nullable&lt;Double&gt;, Nullable&lt;Boolean&gt;, Boolean, Func&lt;TenantOperationMessage, Boolean&gt;)](Microsoft.SharePoint.Client.TenantExtensions.41bc0a90.md) | Sets tenant site Properties
| [SiteExists(Tenant, String)](Microsoft.SharePoint.Client.TenantExtensions.fa3c7d26.md) | Checks if a site collection exists, relies on tenant admin API. Sites that are recycled also return as existing sites
| [SubSiteExists(Tenant, String)](Microsoft.SharePoint.Client.TenantExtensions.488f63fb.md) | Checks if a sub site exists
## See also
- [OfficeDevPnP.Core.Entities.SiteEntity](OfficeDevPnP.Core.Entities.SiteEntity.md)
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)
