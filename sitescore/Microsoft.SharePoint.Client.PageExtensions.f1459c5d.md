# PageExtensions.AddLayoutToWikiPage Method  
 Applies a layout to a wiki page   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddLayoutToWikiPage(this Web web, String folder, WikiPageLayout layout, String page)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### folder  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;System name of the wiki page library - typically sitepages  

  

#### layout  
&emsp;&emsp;Type: [OfficeDevPnP.Core.WikiPageLayout](OfficeDevPnP.Core.WikiPageLayout.md)  
&emsp;&emsp;Wiki page layout to be applied  

  

#### page  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the page that will get a new wiki page layout  

  

### Return Value
Type: void  

## See also
- [PageExtensions](Microsoft.SharePoint.Client.PageExtensions.md) 
- System.ArgumentException
- System.ArgumentNullException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
