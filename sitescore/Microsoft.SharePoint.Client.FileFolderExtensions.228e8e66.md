# FileFolderExtensions.ResolveSubFolder Method  
 Gets a folder with a given name in a given Microsoft.SharePoint.Client.Folder  

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Folder ResolveSubFolder(this Folder folder, String folderName)
```
### Parameters
#### folder  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Folder  
&emsp;&emsp; in which to search for  

  

#### folderName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the folder to search for  

  

### Return Value
Type: Folder  
The found Microsoft.SharePoint.Client.Folder if available, null otherwise  


## See also
- [FileFolderExtensions](Microsoft.SharePoint.Client.FileFolderExtensions.md) 
- Microsoft.SharePoint.Client.Folder
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
