# FileFolderExtensions.EnsureFolder Method  
  

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Folder EnsureFolder(Web web, Folder parentFolder, String folderPath, Expression<Func<Folder, Object>>[] expressions)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;  

  

#### parentFolder  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Folder  
&emsp;&emsp;  

  

#### folderPath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;  

  

#### expressions  
&emsp;&emsp;Type: System.Linq.Expressions.Expression<System.Func<Microsoft.SharePoint.Client.Folder, System.Object>>[]  
&emsp;&emsp;  

  

### Return Value
Type: Folder  

## See also
- [FileFolderExtensions](Microsoft.SharePoint.Client.FileFolderExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
