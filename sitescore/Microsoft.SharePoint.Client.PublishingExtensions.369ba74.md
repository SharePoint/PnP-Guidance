# PublishingExtensions.GetPublishingPage Method  
 Gets a Publishing Page from the root folder of the Pages library.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static PublishingPage GetPublishingPage(this Web web, String fileLeafRef)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The web.  

  

#### fileLeafRef  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The file leaf reference.  

  

### Return Value
Type: PublishingPage  
The PublishingPage object, if any. Otherwise null.  


## See also
- [PublishingExtensions](Microsoft.SharePoint.Client.PublishingExtensions.md) 
- System.ArgumentNullException
- System.ArgumentException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
