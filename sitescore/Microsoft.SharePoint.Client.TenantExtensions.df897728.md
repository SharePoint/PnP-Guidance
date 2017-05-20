# TenantExtensions.IsSiteActive Method  
 Checks if a site collection is Active   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool IsSiteActive(this Tenant tenant, String siteFullUrl)
```
### Parameters
#### tenant  
&emsp;&emsp;Type: Microsoft.Online.SharePoint.TenantAdministration.Tenant  
&emsp;&emsp;A tenant object pointing to the context of a Tenant Administration site  

  

#### siteFullUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;URL to the site collection  

  

### Return Value
Type: bool  
True if active, false if not  


## See also
- [TenantExtensions](Microsoft.SharePoint.Client.TenantExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
