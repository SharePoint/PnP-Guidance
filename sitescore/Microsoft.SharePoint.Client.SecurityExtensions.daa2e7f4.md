# SecurityExtensions.GetAllUniqueRoleAssignments Method  
 Get all unique role assignments for a web object and all its descendents down to document or list item level.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static IEnumerable<RoleAssignmentEntity> GetAllUniqueRoleAssignments(this Web web, Int32 leafBreadthLimit = 2147483647)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The current web object to be processed.  

  

#### (optional) leafBreadthLimit  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Skip further visiting on this branch if the number of child items or documents with unique role assignments exceeded leafBreadthLimit. When setting to 0, the process will stop at list / document library level.  

  

### Return Value
Type: IEnumerable<RoleAssignmentEntity>  
Returns all role assignments  


## See also
- [SecurityExtensions](Microsoft.SharePoint.Client.SecurityExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
