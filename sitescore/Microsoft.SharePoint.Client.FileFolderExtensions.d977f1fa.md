# FileFolderExtensions.FindFiles Method  
 Find files in a specific folder   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static List<File> FindFiles(this Folder folder, String match)
```
### Parameters
#### folder  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Folder  
&emsp;&emsp;The folder to process  

  

#### match  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;a wildcard pattern to match  

  

### Return Value
Type: List<File>  
A list with the found Microsoft.SharePoint.Client.File objects  


## See also
- [FileFolderExtensions](Microsoft.SharePoint.Client.FileFolderExtensions.md) 
- Microsoft.SharePoint.Client.File
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
