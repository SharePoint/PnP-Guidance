# ListExtensions.UpdateListVersioning Method  
 Enable/disable versioning on a list   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void UpdateListVersioning(this Web web, String listName, Boolean enableVersioning, Boolean enableMinorVersioning = True, Boolean updateAndExecuteQuery = True)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### listName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;List to operate on  

  

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
- System.ArgumentException
- System.ArgumentNullException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
