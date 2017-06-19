# PageExtensions.GetWebPartXml Method  
 Gets XML string of a Webpart   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static string GetWebPartXml(this Web web, Guid webPartId, String serverRelativePageUrl)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### webPartId  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;The id of the webpart  

  

#### serverRelativePageUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Server relative url of the page to add the xml to  

  

### Return Value
Type: string  
Returns XML string of a Webpart  


## See also
- [PageExtensions](Microsoft.SharePoint.Client.PageExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
