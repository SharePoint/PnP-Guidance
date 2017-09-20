# FileFolderExtensions.EnsureFolderPath Method  
 Check if a folder exists with the specified path (relative to the web), and if not creates it (inside a list if necessary)   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Folder EnsureFolderPath(this Web web, String webRelativeUrl, params Expression<Func<Folder, Object>>[] expressions)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to check for the specified folder  

  

#### webRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Path to the folder, relative to the web site  

  

#### expressions  
&emsp;&emsp;Type: System.Linq.Expressions.Expression&lt;System.Func&lt;Microsoft.SharePoint.Client.Folder, System.Object&gt;&gt;[]  
&emsp;&emsp;List of lambda expressions of properties to load when retrieving the object  

  

### Return Value
Type: Folder  
The existing or newly created folder  


## Remarks
 If the specified path is inside an existing list, then the folder is created inside that list. 
 Any existing folders are traversed, and then any remaining parts of the path are created as new folders. 
  
## See also
- [FileFolderExtensions](Microsoft.SharePoint.Client.FileFolderExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
