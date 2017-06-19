# PageExtensions.AddLayoutToWikiPage Method  
 Applies a layout to a wiki page   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddLayoutToWikiPage(this Web web, WikiPageLayout layout, String serverRelativePageUrl)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### layout  
&emsp;&emsp;Type: [OfficeDevPnP.Core.WikiPageLayout](OfficeDevPnP.Core.WikiPageLayout.md)  
&emsp;&emsp;Wiki page layout to be applied  

  

#### serverRelativePageUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Server relative url of the page to add the layout to  

  

### Return Value
Type: void  

## See also
- [PageExtensions](Microsoft.SharePoint.Client.PageExtensions.md) 
- System.ArgumentException
- System.ArgumentNullException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
