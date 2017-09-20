# FileFolderExtensions.FindFiles Method  
 Finds files in the web. Can be slow.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static List<File> FindFiles(this Web web, String match)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The web to process  

  

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
