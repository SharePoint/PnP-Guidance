# BrandingExtensions.DeployPageLayout Method  
 Can be used to deploy page layouts to master page gallery. Should be only used with root web of site collection where publishing features are enabled.  

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void DeployPageLayout(this Web web, String sourceFilePath, String title, String description, String associatedContentTypeID, String folderHierarchy = "")
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web as the root site of the publishing site collection  

  

#### sourceFilePath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Full path to the file which will be uploaded  

  

#### title  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Title for the page layout  

  

#### description  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Description for the page layout  

  

#### associatedContentTypeID  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Associated content type ID  

  

#### (optional) folderHierarchy  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Folder hierarchy where the page layouts will be deployed  

  

### Return Value
Type: void  

## Remarks
Should be only used with root web of site collection where publishing features are enabled.
  
## See also
- [BrandingExtensions](Microsoft.SharePoint.Client.BrandingExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
