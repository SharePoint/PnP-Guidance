# SecurityExtensions.AddAdministrators Method  
 Add a site collection administrator to a site collection   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddAdministrators(this Web web, List<UserEntity> adminLogins, Boolean addToOwnersGroup = False)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to operate on  

  

#### adminLogins  
&emsp;&emsp;Type: System.Collections.Generic.List&lt;OfficeDevPnP.Core.Entities.UserEntity&gt;  
&emsp;&emsp;Array of admins loginnames to add  

  

#### (optional) addToOwnersGroup  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Optionally the added admins can also be added to the Site owners group  

  

### Return Value
Type: void  

## See also
- [SecurityExtensions](Microsoft.SharePoint.Client.SecurityExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
