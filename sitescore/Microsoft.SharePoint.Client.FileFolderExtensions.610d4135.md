# FileFolderExtensions.FindFiles Method  
 Find files in the list, Can be slow.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static List<File> FindFiles(this List list, String match)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;The list to process  

  

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
