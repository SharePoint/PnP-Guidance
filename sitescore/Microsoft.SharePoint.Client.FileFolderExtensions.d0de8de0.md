# FileFolderExtensions.VerifyIfUploadRequired Method  
 Used to compare the server file to the local file. This enables users with faster download speeds but slow upload speeds to evaluate if the server file should be overwritten.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool VerifyIfUploadRequired(this File serverFile, String localFile)
```
### Parameters
#### serverFile  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.File  
&emsp;&emsp;File located on the server.  

  

#### localFile  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;File to validate against.  

  

### Return Value
Type: bool  

## See also
- [FileFolderExtensions](Microsoft.SharePoint.Client.FileFolderExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
