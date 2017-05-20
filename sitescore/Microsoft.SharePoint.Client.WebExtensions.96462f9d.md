# WebExtensions.SiteSearch Method  
 Returns all site collections that are indexed. In MT the search center, mysite host and contenttype hub are defined as non indexable by default and thus are not returned   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static List<SiteEntity> SiteSearch(this Web web)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

### Return Value
Type: List<SiteEntity>  
All site collections  


## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
