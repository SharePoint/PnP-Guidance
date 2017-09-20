# JavaScriptExtensions.AddJsBlock Method  
 Injects javascript via a adding a custom action to the site   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool AddJsBlock(this Web web, String key, String scriptBlock, Int32 sequence = 0)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### key  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Identifier (key) for the custom action that will be created  

  

#### scriptBlock  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Javascript to be injected  

  

#### (optional) sequence  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Specifies the ordering priority for actions. A value is 0 indicates that the button will appear at the first position on the ribbon.  

  

### Return Value
Type: bool  
True if action was ok  


## See also
- [JavaScriptExtensions](Microsoft.SharePoint.Client.JavaScriptExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
