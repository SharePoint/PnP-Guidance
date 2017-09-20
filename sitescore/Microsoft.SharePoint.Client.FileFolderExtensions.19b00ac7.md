# FileFolderExtensions.ConvertFolderToDocumentSet Method  
 Converts a folder with the given name as a child of the List RootFolder.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Folder ConvertFolderToDocumentSet(this List list, Folder folder)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;List in which the folder exists  

  

#### folder  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Folder  
&emsp;&emsp;Folder to convert  

  

### Return Value
Type: Folder  
The newly converted Document Set, so that additional operations (such as setting properties) can be done.  


## Remarks
 Note that this only checks one level of folder (the Folders collection) and cannot accept a name with path characters. 
  
## See also
- [FileFolderExtensions](Microsoft.SharePoint.Client.FileFolderExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
