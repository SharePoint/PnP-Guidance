# TenantExtensions.AddAdministrators Method  
 Add a site collection administrator to a site collection   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddAdministrators(this Tenant tenant, IEnumerable<UserEntity> adminLogins, Uri siteUrl, Boolean addToOwnersGroup = False)
```
### Parameters
#### tenant  
&emsp;&emsp;Type: Microsoft.Online.SharePoint.TenantAdministration.Tenant  
&emsp;&emsp;A tenant object pointing to the context of a Tenant Administration site  

  

#### adminLogins  
&emsp;&emsp;Type: System.Collections.Generic.IEnumerable&lt;OfficeDevPnP.Core.Entities.UserEntity&gt;  
&emsp;&emsp;Array of admins loginnames to add  

  

#### siteUrl  
&emsp;&emsp;Type: System.Uri  
&emsp;&emsp;Url of the site to operate on  

  

#### (optional) addToOwnersGroup  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Optionally the added admins can also be added to the Site owners group  

  

### Return Value
Type: void  

## See also
- [TenantExtensions](Microsoft.SharePoint.Client.TenantExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
