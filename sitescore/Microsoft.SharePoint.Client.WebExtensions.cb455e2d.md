# WebExtensions.UninstallSolution Method  
 Uninstalls a sandbox solution package (.WSP) file   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void UninstallSolution(this Site site, Guid packageGuid, String fileName, Int32 majorVersion = 1, Int32 minorVersion = 0)
```
### Parameters
#### site  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Site  
&emsp;&emsp;Site collection to install to  

  

#### packageGuid  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;ID of the solution, from the solution manifest  

  

#### fileName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;filename of the WSP file to uninstall  

  

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
