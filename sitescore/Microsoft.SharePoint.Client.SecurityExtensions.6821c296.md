# SecurityExtensions.AddGroup Method  
 Adds a group   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Group AddGroup(this Web web, String groupName, String groupDescription, Boolean groupIsOwner, Boolean updateAndExecuteQuery = True, Boolean onlyAllowMembersViewMembership = False)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to add the group to  

  

#### groupName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the group  

  

#### groupDescription  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Description of the group  

  

#### groupIsOwner  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Sets the created group as group owner if true  

  

#### (optional) updateAndExecuteQuery  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Set to false to postpone the executequery call  

  

#### (optional) onlyAllowMembersViewMembership  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Set whether members are allowed to see group membership, defaults to false  

  

### Return Value
Type: Group  
The created group  


## See also
- [SecurityExtensions](Microsoft.SharePoint.Client.SecurityExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
