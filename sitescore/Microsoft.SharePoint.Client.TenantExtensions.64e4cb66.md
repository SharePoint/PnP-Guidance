# TenantExtensions.GetSiteGuidByUrl Method  
 Gets the ID of site collection with specified URL   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Guid GetSiteGuidByUrl(this Tenant tenant, Uri siteFullUrl)
```
### Parameters
#### tenant  
&emsp;&emsp;Type: Microsoft.Online.SharePoint.TenantAdministration.Tenant  
&emsp;&emsp;A tenant object pointing to the context of a Tenant Administration site  

  

#### siteFullUrl  
&emsp;&emsp;Type: System.Uri  
&emsp;&emsp;A URL that specifies a site collection to get ID.  

  

### Return Value
Type: Guid  
The Guid of a site collection or an Guid.Empty if the Site does not exist  


## See also
- [TenantExtensions](Microsoft.SharePoint.Client.TenantExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
