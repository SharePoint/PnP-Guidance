# SecurityExtensions.RemovePermissionLevelFromUser Method  
 Removes a permission level from a user   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void RemovePermissionLevelFromUser(this SecurableObject securableObject, String userLoginName, String roleDefinitionName, Boolean removeAllPermissionLevels = False)
```
### Parameters
#### securableObject  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.SecurableObject  
&emsp;&emsp;Web/List/Item to operate against  

  

#### userLoginName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Loginname of user  

  

#### roleDefinitionName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the role definition to add, Full Control|Design|Contribute|Read|Approve|Manage Heirarchy|Restricted Read. Use the correct name of the language of the site you are using  

  

#### (optional) removeAllPermissionLevels  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Set to true to remove all permission level.  

  

### Return Value
Type: void  

## See also
- [SecurityExtensions](Microsoft.SharePoint.Client.SecurityExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
