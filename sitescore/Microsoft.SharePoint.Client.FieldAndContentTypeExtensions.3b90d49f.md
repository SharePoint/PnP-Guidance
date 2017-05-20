# FieldAndContentTypeExtensions.ContentTypeExistsByName Method  
 Does content type exists in the web   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool ContentTypeExistsByName(this Web web, String contentTypeName, Boolean searchInSiteHierarchy = False)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to be processed  

  

#### contentTypeName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the content type  

  

#### (optional) searchInSiteHierarchy  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Searches accross all content types in the site up to the root site  

  

### Return Value
Type: bool  
True if the content type exists, false otherwise  


## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
