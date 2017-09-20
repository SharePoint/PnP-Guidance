# WebExtensions.DeleteWeb Method  
 Deletes the child website with the specified leaf URL, from a parent Web, if it exists.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool DeleteWeb(this Web parentWeb, String leafUrl)
```
### Parameters
#### parentWeb  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The parent Web (site) to delete from  

  

#### leafUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;A string that represents the URL leaf name.  

  

### Return Value
Type: bool  
true if the web was deleted; otherwise false if nothing was done  


## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
