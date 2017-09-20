# BrandingExtensions.DeployMasterPage Method  
 Deploys a new masterpage   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static File DeployMasterPage(this Web web, String sourceFilePath, String title, String description, String uiVersion = "15", String defaultCSSFile = "", String folderPath = "")
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The web to process  

  

#### sourceFilePath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The path to the source file  

  

#### title  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The title of the masterpage  

  

#### description  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The description of the masterpage  

  

#### (optional) uiVersion  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;UIVersion of the masterpage  

  

#### (optional) defaultCSSFile  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;DefaultCSSFile of the masterpage  

  

#### (optional) folderPath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;FolderPath of the masterpage  

  

### Return Value
Type: File  

## See also
- [BrandingExtensions](Microsoft.SharePoint.Client.BrandingExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
