# ListExtensions.CreateDocumentLibrary Method  
 Adds a document library to a web. Execute Query is called during this implementation   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static List CreateDocumentLibrary(this Web web, String listName, Boolean enableVersioning = False, String urlPath = "")
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### listName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the library  

  

#### (optional) enableVersioning  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Enable versioning on the list  

  

#### (optional) urlPath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Path of the url  

  

### Return Value
Type: List  

## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- System.ArgumentException
- System.ArgumentNullException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
