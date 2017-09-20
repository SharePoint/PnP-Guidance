# FileFolderExtensions.SaveFileToLocal Method  
 Saves a remote file to a local folder   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SaveFileToLocal(this Web web, String serverRelativeUrl, String localPath, String localFileName, Func<String, Boolean> fileExistsCallBack)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The Web to process  

  

#### serverRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The server relative url to the file  

  

#### localPath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The local folder  

  

#### (optional) localFileName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The local filename. If null the filename of the file on the server will be used  

  

#### (optional) fileExistsCallBack  
&emsp;&emsp;Type: System.Func&lt;System.String, System.Boolean&gt;  
&emsp;&emsp;Optional callback function allowing to provide feedback if the file should be overwritten if it exists. The function requests a bool as return value and the string input contains the name of the file that exists.  

  

### Return Value
Type: void  

## See also
- [FileFolderExtensions](Microsoft.SharePoint.Client.FileFolderExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
