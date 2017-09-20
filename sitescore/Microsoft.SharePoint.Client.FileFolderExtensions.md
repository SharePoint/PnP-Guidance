# FileFolderExtensions Class
 Class that holds the deprecated file and folder methods   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class FileFolderExtensions
```
## Extension Methods
|**Name**|**Description**|
|:-----|:-----|
| [ApproveFile(Web, String, String)](Microsoft.SharePoint.Client.FileFolderExtensions.ab86a84b.md) | Approves a file
| [CheckInFile(Web, String, CheckinType, String)](Microsoft.SharePoint.Client.FileFolderExtensions.c0c23a8a.md) | Checks in a file
| [CheckOutFile(Web, String)](Microsoft.SharePoint.Client.FileFolderExtensions.777298ba.md) | Checks out a file
| [ConvertFolderToDocumentSet(List, String)](Microsoft.SharePoint.Client.FileFolderExtensions.b1ee8b29.md) | Converts a folder with the given name as a child of the List RootFolder.
| [ConvertFolderToDocumentSet(List, Folder)](Microsoft.SharePoint.Client.FileFolderExtensions.19b00ac7.md) | Converts a folder with the given name as a child of the List RootFolder.
| [CreateDocumentSet(Folder, String, ContentTypeId)](Microsoft.SharePoint.Client.FileFolderExtensions.cceeb4a1.md) | Creates a new document set as a child of an existing folder, with the specified content type ID.
| [CreateFolder(Web, String)](Microsoft.SharePoint.Client.FileFolderExtensions.5a3cbd57.md) | Creates a folder with the given name as a child of the Web. Note it is more common to create folders within an existing Folder, such as the RootFolder of a List.
| [CreateFolder(Folder, String)](Microsoft.SharePoint.Client.FileFolderExtensions.2d34edc8.md) | Creates a folder with the given name.
| [DoesFolderExists(Web, String)](Microsoft.SharePoint.Client.FileFolderExtensions.f242ff96.md) | Checks if a specific folder exists
| [EnsureFolder(Web, Folder, String, Expression&lt;Func&lt;Folder, Object&gt;&gt;[])](Microsoft.SharePoint.Client.FileFolderExtensions.ff1bc66d.md) | Ensure that the folder structure is created. This also ensures hierarchy of folders.
| [EnsureFolder(Web, String, Expression&lt;Func&lt;Folder, Object&gt;&gt;[])](Microsoft.SharePoint.Client.FileFolderExtensions.f0af8f8.md) | Checks if the folder exists at the top level of the web site, and if it does not exist creates it. Note it is more common to create folders within an existing Folder, such as the RootFolder of a List.
| [EnsureFolder(Folder, String, Expression&lt;Func&lt;Folder, Object&gt;&gt;[])](Microsoft.SharePoint.Client.FileFolderExtensions.cb4683a9.md) | Checks if the subfolder exists, and if it does not exist creates it.
| [EnsureFolderPath(Web, String, Expression&lt;Func&lt;Folder, Object&gt;&gt;[])](Microsoft.SharePoint.Client.FileFolderExtensions.35b06e1c.md) | Check if a folder exists with the specified path (relative to the web), and if not creates it (inside a list if necessary)
| [FindFiles(Web, String)](Microsoft.SharePoint.Client.FileFolderExtensions.9355c7ca.md) | Finds files in the web. Can be slow.
| [FindFiles(List, String)](Microsoft.SharePoint.Client.FileFolderExtensions.610d4135.md) | Find files in the list, Can be slow.
| [FindFiles(Folder, String)](Microsoft.SharePoint.Client.FileFolderExtensions.d977f1fa.md) | Find files in a specific folder
| [FolderExists(Web, String)](Microsoft.SharePoint.Client.FileFolderExtensions.e44be55d.md) | Checks if the folder exists at the top level of the web site.
| [FolderExists(Folder, String)](Microsoft.SharePoint.Client.FileFolderExtensions.d7370e83.md) | Checks if the subfolder exists.
| [GetFile(Folder, String)](Microsoft.SharePoint.Client.FileFolderExtensions.68f7e2cb.md) | Gets a file in a document library.
| [GetFileAsString(Web, String)](Microsoft.SharePoint.Client.FileFolderExtensions.cccf4e5b.md) | Returns a file as string
| [PublishFile(Web, String, String)](Microsoft.SharePoint.Client.FileFolderExtensions.1c9a167d.md) | Publishes a file existing on a server url
| [PublishFileToLevel(File, FileLevel)](Microsoft.SharePoint.Client.FileFolderExtensions.be85f58d.md) | Publishes a file based on the type of versioning required on the parent library.
| [ResolveSubFolder(Folder, String)](Microsoft.SharePoint.Client.FileFolderExtensions.228e8e66.md) |  Gets a folder with a given name in a given Microsoft.SharePoint.Client.Folder 
| [SaveFileToLocal(Web, String, String, String, Func&lt;String, Boolean&gt;)](Microsoft.SharePoint.Client.FileFolderExtensions.b94118ad.md) | Saves a remote file to a local folder
| [SetFileProperties(File, IDictionary&lt;String, String&gt;, Boolean)](Microsoft.SharePoint.Client.FileFolderExtensions.dc97957.md) | Sets file properties using a dictionary.
| [UploadFile(Folder, String, String, Boolean)](Microsoft.SharePoint.Client.FileFolderExtensions.4188915.md) | Uploads a file to the specified folder.
| [UploadFile(Folder, String, Stream, Boolean)](Microsoft.SharePoint.Client.FileFolderExtensions.203708bc.md) | Uploads a file to the specified folder.
| [UploadFileWebDav(Folder, String, String, Boolean)](Microsoft.SharePoint.Client.FileFolderExtensions.49dc7cad.md) | Uploads a file to the specified folder by saving the binary directly (via webdav).
| [UploadFileWebDav(Folder, String, Stream, Boolean)](Microsoft.SharePoint.Client.FileFolderExtensions.2a46b076.md) | Uploads a file to the specified folder by saving the binary directly (via webdav). Note: this method does not work using app only token.
| [VerifyIfUploadRequired(File, String)](Microsoft.SharePoint.Client.FileFolderExtensions.d0de8de0.md) | Used to compare the server file to the local file. This enables users with faster download speeds but slow upload speeds to evaluate if the server file should be overwritten.
| [VerifyIfUploadRequired(File, Stream)](Microsoft.SharePoint.Client.FileFolderExtensions.16cba753.md) | Used to compare the server file to the local file. This enables users with faster download speeds but slow upload speeds to evaluate if the server file should be overwritten.
## See also
- Microsoft.SharePoint.Client.File
- Microsoft.SharePoint.Client.Folder
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)
