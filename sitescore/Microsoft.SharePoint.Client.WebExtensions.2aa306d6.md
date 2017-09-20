# WebExtensions.SiteSearchScopedByUrl Method  
 Returns all site collection that start with the provided URL   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static List<SiteEntity> SiteSearchScopedByUrl(this Web web, String siteUrl)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### siteUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Base URL for which sites can be returned  

  

### Return Value
Type: List<SiteEntity>  
All found site collections  


## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
