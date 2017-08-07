# WebExtensions.SiteSearch Method  
 Returns the site collections that comply with the passed keyword query   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static List<SiteEntity> SiteSearch(this Web web, String keywordQueryValue, Boolean trimDuplicates = False)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### keywordQueryValue  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Keyword query  

  

#### (optional) trimDuplicates  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Indicates if duplicates should be trimmed or not  

  

### Return Value
Type: List<SiteEntity>  
All found site collections  


## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
