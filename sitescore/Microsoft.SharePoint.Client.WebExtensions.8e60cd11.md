# WebExtensions.InstallSolution Method  
 Uploads and installs a sandbox solution package (.WSP) file, replacing existing solution if necessary.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void InstallSolution(this Site site, Guid packageGuid, String sourceFilePath, Int32 majorVersion = 1, Int32 minorVersion = 0)
```
### Parameters
#### site  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Site  
&emsp;&emsp;Site collection to install to  

  

#### packageGuid  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;ID of the solution, from the solution manifest (required for the remove step)  

  

#### sourceFilePath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Path to the sandbox solution package (.WSP) file  

  

#### (optional) majorVersion  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Optional major version of the solution, defaults to 1  

  

#### (optional) minorVersion  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Optional minor version of the solution, defaults to 0  

  

### Return Value
Type: void  

## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
