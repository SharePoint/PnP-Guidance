# ListExtensions.CreateList Method  
 Adds a custom list to a site   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static List CreateList(this Web web, Guid featureId, Int32 listType, String listName, Boolean enableVersioning, Boolean updateAndExecuteQuery = True, String urlPath = "", Boolean enableContentTypes = False)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### featureId  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;Feature that contains the list template  

  

#### listType  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Type ID of the list, within the feature  

  

#### listName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the list  

  

#### enableVersioning  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Enable versioning on the list  

  

#### (optional) updateAndExecuteQuery  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;(Optional) Perform list update and executequery, defaults to true  

  

#### (optional) urlPath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;(Optional) URL to use for the list  

  

#### (optional) enableContentTypes  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;(Optional) Enable content type management  

  

### Return Value
Type: List  
The newly created list  


## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
