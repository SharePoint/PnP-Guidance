# PageExtensions.AddHtmlToWikiPage Method  
 Add a HTML fragment to a location on a wiki style page   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddHtmlToWikiPage(this Web web, String serverRelativePageUrl, String html, Int32 row, Int32 col)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### serverRelativePageUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;server relative Url of the page to add the fragment to  

  

#### html  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;html to be inserted  

  

#### row  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Row of the wiki table that should hold the inserted web part  

  

#### col  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Column of the wiki table that should hold the inserted web part  

  

### Return Value
Type: void  

## See also
- [PageExtensions](Microsoft.SharePoint.Client.PageExtensions.md) 
- System.ArgumentException
- System.ArgumentNullException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
