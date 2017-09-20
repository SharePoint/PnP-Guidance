# WebExtensions.IsNoScriptSite Method  
 Detects if the site in question has no script enabled or not. Detection is done by verifying if the AddAndCustomizePages permission is missing. See https://support.office.com/en-us/article/Turn-scripting-capabilities-on-or-off-1f2c515f-5d7e-448a-9fd7-835da935584f for the effects of NoScript   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool IsNoScriptSite(this Site site)
```
### Parameters
#### site  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Site  
&emsp;&emsp;site to verify  

  

### Return Value
Type: bool  
True if noscript, false otherwise  


## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
