# WebExtensions.WebExists Method  
 Determines if a child Web site with the specified leaf URL exists.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool WebExists(this Web parentWeb, String leafUrl)
```
### Parameters
#### parentWeb  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The Web site to check under  

  

#### leafUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;A string that represents the URL leaf name.  

  

### Return Value
Type: bool  
true if the Web (site) exists; otherwise false  


## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
