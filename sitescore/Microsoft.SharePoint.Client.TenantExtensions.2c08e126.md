# TenantExtensions.GetOneDriveSiteCollections Method  
 Get OneDrive site collections by iterating through all user profiles.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static IList<SiteEntity> GetOneDriveSiteCollections(this Tenant tenant)
```
### Parameters
#### tenant  
&emsp;&emsp;Type: Microsoft.Online.SharePoint.TenantAdministration.Tenant  
&emsp;&emsp;A tenant object pointing to the context of a Tenant Administration site   

  

### Return Value
Type: IList<SiteEntity>  
List of  [OfficeDevPnP.Core.Entities.SiteEntity](OfficeDevPnP.Core.Entities.SiteEntity.md)  objects containing site collection info  


## See also
- [TenantExtensions](Microsoft.SharePoint.Client.TenantExtensions.md) 
- [OfficeDevPnP.Core.Entities.SiteEntity](OfficeDevPnP.Core.Entities.SiteEntity.md)
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
