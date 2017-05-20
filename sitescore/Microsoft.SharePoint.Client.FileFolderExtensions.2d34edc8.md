# FileFolderExtensions.CreateFolder Method  
 Creates a folder with the given name.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Folder CreateFolder(this Folder parentFolder, String folderName)
```
### Parameters
#### parentFolder  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Folder  
&emsp;&emsp;Parent folder to create under  

  

#### folderName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Folder name to retrieve or create  

  

### Return Value
Type: Folder  
The newly created folder  


## Remarks
 Note that this only checks one level of folder (the Folders collection) and cannot accept a name with path characters. 

```C#
var folder = list.RootFolder.CreateFolder("new-folder");
            
```
  
## See also
- [FileFolderExtensions](Microsoft.SharePoint.Client.FileFolderExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
