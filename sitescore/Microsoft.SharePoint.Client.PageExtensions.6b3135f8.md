# PageExtensions.AddHtmlToWikiPage Method  
 Add html to a wiki style page   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddHtmlToWikiPage(this Web web, String folder, String html, String page)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### folder  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;System name of the wiki page library - typically sitepages  

  

#### html  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The html to insert  

  

#### page  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Page to add the html on  

  

### Return Value
Type: void  

## See also
- [PageExtensions](Microsoft.SharePoint.Client.PageExtensions.md) 
- System.ArgumentException
- System.ArgumentNullException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
