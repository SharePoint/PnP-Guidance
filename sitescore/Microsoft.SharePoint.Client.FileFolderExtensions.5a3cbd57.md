# FileFolderExtensions.CreateFolder Method  
 Creates a folder with the given name as a child of the Web. Note it is more common to create folders within an existing Folder, such as the RootFolder of a List.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Folder CreateFolder(this Web web, String folderName)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to check for the named folder  

  

#### folderName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Folder name to retrieve or create  

  

### Return Value
Type: Folder  
The newly created Folder, so that additional operations (such as setting properties) can be done.  


## Remarks
 Note that this only checks one level of folder (the Folders collection) and cannot accept a name with path characters. 
  
## See also
- [FileFolderExtensions](Microsoft.SharePoint.Client.FileFolderExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
