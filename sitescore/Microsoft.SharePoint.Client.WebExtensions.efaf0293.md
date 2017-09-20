# WebExtensions.EnableRequestAccess Method  
 Enables request access for the specified e-mail addresses.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void EnableRequestAccess(this Web web, IEnumerable<String> emails)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The web to enable request access.  

  

#### emails  
&emsp;&emsp;Type: System.Collections.Generic.IEnumerable&lt;System.String&gt;  
&emsp;&emsp;The e-mail addresses to send access requests to.  

  

### Return Value
Type: void  

## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
