# BrandingExtensions.UploadThemeFile Method  
 Uploads the specified file (usually an spcolor or spfont file) to the web site themes gallery (usually only exists in the root web of a site collection).   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static File UploadThemeFile(this Web web, String localFilePath, String themeFolderVersion = "15")
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web site to upload to  

  

#### localFilePath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Location of the file to be uploaded  

  

#### (optional) themeFolderVersion  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Leaf folder name to upload to; default is "15"  

  

### Return Value
Type: File  
The uploaded file, with at least the ServerRelativeUrl property available  


## See also
- [BrandingExtensions](Microsoft.SharePoint.Client.BrandingExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
