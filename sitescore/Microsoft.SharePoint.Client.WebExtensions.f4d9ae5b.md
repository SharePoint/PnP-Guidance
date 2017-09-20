# WebExtensions.GetWeb Method  
 Returns the child Web site with the specified leaf URL.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Web GetWeb(this Web parentWeb, String leafUrl)
```
### Parameters
#### parentWeb  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The Web site to check under  

  

#### leafUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;A string that represents the URL leaf name.  

  

### Return Value
Type: Web  
The requested Web, if it exists, otherwise null.  


## Remarks
 The ServerRelativeUrl property of the retrieved Web is instantiated. 
  
## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
