# SecurityExtensions.RemovePermissionLevelFromGroup Method  
 Removes a permission level from a group   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void RemovePermissionLevelFromGroup(this SecurableObject securableObject, String groupName, RoleType permissionLevel, Boolean removeAllPermissionLevels = False)
```
### Parameters
#### securableObject  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.SecurableObject  
&emsp;&emsp;Web/List/Item to operate against  

  

#### groupName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;name of the group  

  

#### permissionLevel  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.RoleType  
&emsp;&emsp;Permission level to remove. If null all permission levels are removed  

  

#### (optional) removeAllPermissionLevels  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Set to true to remove all permission level.  

  

### Return Value
Type: void  

## See also
- [SecurityExtensions](Microsoft.SharePoint.Client.SecurityExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
