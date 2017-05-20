# TenantExtensions.CheckIfSiteExists Method  
 Returns if a site collection is in a particular status. If the url contains a sub site then returns true is the sub site exists, false if not. Status is irrelevant for sub sites   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool CheckIfSiteExists(this Tenant tenant, String siteFullUrl, String status)
```
### Parameters
#### tenant  
&emsp;&emsp;Type: Microsoft.Online.SharePoint.TenantAdministration.Tenant  
&emsp;&emsp;A tenant object pointing to the context of a Tenant Administration site  

  

#### siteFullUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Url to the site collection  

  

#### status  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Status to check (Active, Creating, Recycled)  

  

### Return Value
Type: bool  
True if in status, false if not in status  


## See also
- [TenantExtensions](Microsoft.SharePoint.Client.TenantExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
