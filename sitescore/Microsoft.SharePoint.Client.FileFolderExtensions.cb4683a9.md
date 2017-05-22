# FileFolderExtensions.EnsureFolder Method  
 Checks if the subfolder exists, and if it does not exist creates it.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Folder EnsureFolder(this Folder parentFolder, String folderName, params Expression<Func<Folder, Object>>[] expressions)
```
### Parameters
#### parentFolder  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Folder  
&emsp;&emsp;Parent folder to create under  

  

#### folderName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Folder name to retrieve or create  

  

#### expressions  
&emsp;&emsp;Type: System.Linq.Expressions.Expression&lt;System.Func&lt;Microsoft.SharePoint.Client.Folder, System.Object&gt;&gt;[]  
&emsp;&emsp;List of lambda expressions of properties to load when retrieving the object  

  

### Return Value
Type: Folder  
The existing or newly created folder  


## Remarks
 Note that this only checks one level of folder (the Folders collection) and cannot accept a name with path characters. 
  
## See also
- [FileFolderExtensions](Microsoft.SharePoint.Client.FileFolderExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
