# FileFolderExtensions.FolderExists Method  
 Checks if the subfolder exists.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool FolderExists(this Folder parentFolder, String folderName)
```
### Parameters
#### parentFolder  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Folder  
&emsp;&emsp;Parent folder to check for the named subfolder  

  

#### folderName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Folder name to retrieve  

  

### Return Value
Type: bool  
true if the folder exists; false otherwise  


## Remarks
 Note that this only checks one level of folder (the Folders collection) and cannot accept a name with path characters. 
  
## See also
- [FileFolderExtensions](Microsoft.SharePoint.Client.FileFolderExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
