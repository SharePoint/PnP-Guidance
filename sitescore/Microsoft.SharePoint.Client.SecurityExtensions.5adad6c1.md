# SecurityExtensions.AddPermissionLevelToUser Method  
 Add a permission level (e.g.Contribute, Reader,...) to a user   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddPermissionLevelToUser(this SecurableObject securableObject, String userLoginName, RoleType permissionLevel, Boolean removeExistingPermissionLevels = False)
```
### Parameters
#### securableObject  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.SecurableObject  
&emsp;&emsp;Web/List/Item to operate against  

  

#### userLoginName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Loginname of the user  

  

#### permissionLevel  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.RoleType  
&emsp;&emsp;Permission level to add  

  

#### (optional) removeExistingPermissionLevels  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Set to true to remove all other permission levels for that user  

  

### Return Value
Type: void  

## See also
- [SecurityExtensions](Microsoft.SharePoint.Client.SecurityExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
