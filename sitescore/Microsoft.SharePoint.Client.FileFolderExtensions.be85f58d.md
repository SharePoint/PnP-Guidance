# FileFolderExtensions.PublishFileToLevel Method  
 Publishes a file based on the type of versioning required on the parent library.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void PublishFileToLevel(this File file, FileLevel level)
```
### Parameters
#### file  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.File  
&emsp;&emsp;Target file to publish.  

  

#### level  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.FileLevel  
&emsp;&emsp;Target publish direction (Draft and Published only apply, Checkout is ignored).  

  

### Return Value
Type: void  

## See also
- [FileFolderExtensions](Microsoft.SharePoint.Client.FileFolderExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
