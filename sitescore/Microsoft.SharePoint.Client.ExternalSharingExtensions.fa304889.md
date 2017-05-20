# ExternalSharingExtensions.UnshareDocument Method  
 Can be used to programatically to unshare any document with the document URL.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static SharingResult UnshareDocument(this Web web, String urlToDocument)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web for the context used for people picker search  

  

#### urlToDocument  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Full URL to the file which is shared  

  

### Return Value
Type: SharingResult  

## See also
- [ExternalSharingExtensions](Microsoft.SharePoint.Client.ExternalSharingExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
