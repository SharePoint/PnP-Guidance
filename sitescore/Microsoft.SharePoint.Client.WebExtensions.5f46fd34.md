# WebExtensions.WebExistsFullUrl Method  
 Determines if a Web (site) exists at the specified full URL, either accessible or that returns an access error.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool WebExistsFullUrl(this ClientRuntimeContext context, String webFullUrl)
```
### Parameters
#### context  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ClientRuntimeContext  
&emsp;&emsp;Existing context, used to provide credentials.  

  

#### webFullUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Full URL of the site to check.  

  

### Return Value
Type: bool  
true if the Web (site) exists; otherwise false  


## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
