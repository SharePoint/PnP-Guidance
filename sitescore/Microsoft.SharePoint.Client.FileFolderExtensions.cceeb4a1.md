# FileFolderExtensions.CreateDocumentSet Method  
 Creates a new document set as a child of an existing folder, with the specified content type ID.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Folder CreateDocumentSet(Folder folder, String documentSetName, ContentTypeId contentTypeId)
```
### Parameters
#### folder  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Folder  
&emsp;&emsp; Creates a new document set as a child of an existing folder, with the specified content type ID.   

  

#### documentSetName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp; Creates a new document set as a child of an existing folder, with the specified content type ID.   

  

#### contentTypeId  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ContentTypeId  
&emsp;&emsp;Content type of the document set  

  

### Return Value
Type: Folder  
The created Folder representing the document set, so that additional operations (such as setting properties) can be done.  


## Remarks

```C#
var setContentType = list.BestMatchContentTypeId(BuiltInContentTypeId.DocumentSet);
var set1 = list.RootFolder.CreateDocumentSet("Set 1", setContentType);
            
```
  
## See also
- [FileFolderExtensions](Microsoft.SharePoint.Client.FileFolderExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
