# SecurityExtensions.AddPermissionLevelToUser Method  
 Add a role definition (e.g.Contribute, Read, Approve) to a user   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddPermissionLevelToUser(this SecurableObject securableObject, String userLoginName, String roleDefinitionName, Boolean removeExistingPermissionLevels = False)
```
### Parameters
#### securableObject  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.SecurableObject  
&emsp;&emsp;Web/List/Item to operate against  

  

#### userLoginName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Loginname of the user  

  

#### roleDefinitionName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the role definition to add, Full Control|Design|Contribute|Read|Approve|Manage Hierarchy|Restricted Read. Use the correct name of the language of the root site you are using  

  

#### (optional) removeExistingPermissionLevels  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Set to true to remove all other permission levels for that user  

  

### Return Value
Type: void  

## See also
- [SecurityExtensions](Microsoft.SharePoint.Client.SecurityExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
