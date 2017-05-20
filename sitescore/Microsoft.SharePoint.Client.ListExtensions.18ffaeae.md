# ListExtensions.ListExists Method  
 Checks if list exists on the particular site based on the list's site relative path.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool ListExists(this Web web, Uri siteRelativeUrlPath)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### siteRelativeUrlPath  
&emsp;&emsp;Type: System.Uri  
&emsp;&emsp;Site relative path of the list  

  

### Return Value
Type: bool  
True if the list exists  


## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
