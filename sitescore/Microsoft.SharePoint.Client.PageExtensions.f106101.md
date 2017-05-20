# PageExtensions.AddHtmlToWikiPage Method  
 Add a HTML fragment to a location on a wiki style page   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddHtmlToWikiPage(this Web web, String folder, String html, String page, Int32 row, Int32 col)
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
&emsp;&emsp;html to be inserted  

  

#### page  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Page to add the web part on  

  

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
