# ListExtensions.UpdateListVersioning Method  
 Enable/disable versioning on a list   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void UpdateListVersioning(this List list, Boolean enableVersioning, Boolean enableMinorVersioning = True, Boolean updateAndExecuteQuery = True)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;List to be processed  

  

#### enableVersioning  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;True to enable versioning, false to disable  

  

#### (optional) enableMinorVersioning  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Enable/Disable minor versioning  

  

#### (optional) updateAndExecuteQuery  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Perform list update and executequery, defaults to true  

  

### Return Value
Type: void  

## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
