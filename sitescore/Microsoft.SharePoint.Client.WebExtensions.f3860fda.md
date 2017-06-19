# WebExtensions.GetEventReceiverByName Method  
 Returns an event receiver definition   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static EventReceiverDefinition GetEventReceiverByName(this Web web, String name)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to process  

  

#### name  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The name of the receiver  

  

### Return Value
Type: EventReceiverDefinition  
Returns an EventReceiverDefinition if succeeded. Returns null if failed.  


## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
