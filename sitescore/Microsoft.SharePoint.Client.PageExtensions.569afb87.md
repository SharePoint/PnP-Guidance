# PageExtensions.DeleteWebPart Method  
 Deletes a web part from a page   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void DeleteWebPart(this Web web, String folder, String title, String page)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### folder  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;System name of the wiki page library - typically sitepages  

  

#### title  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Title of the web part that needs to be deleted  

  

#### page  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Page to remove the web part from  

  

### Return Value
Type: void  

## See also
- [PageExtensions](Microsoft.SharePoint.Client.PageExtensions.md) 
- System.ArgumentException
- System.ArgumentNullException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
