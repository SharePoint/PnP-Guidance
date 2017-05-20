# JavaScriptExtensions.DeleteJsLink Method  
 Removes the custom action that triggers the execution of a javascript link   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool DeleteJsLink(this Web web, String key)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### key  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Identifier (key) for the custom action that will be deleted  

  

### Return Value
Type: bool  
True if action was ok  


## See also
- [JavaScriptExtensions](Microsoft.SharePoint.Client.JavaScriptExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
