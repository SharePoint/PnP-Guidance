# PageExtensions.AddWikiPageByUrl Method  
 Adds a wiki page by Url   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddWikiPageByUrl(this Web web, String serverRelativePageUrl, String html)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The web to process  

  

#### serverRelativePageUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Server relative URL of the wiki page to process  

  

#### (optional) html  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;HTML to add to wiki page  

  

### Return Value
Type: void  

## See also
- [PageExtensions](Microsoft.SharePoint.Client.PageExtensions.md) 
- System.ArgumentException
- System.ArgumentNullException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
