# WebExtensions.GetEventReceiverById Method  
 Returns an event receiver definition   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static EventReceiverDefinition GetEventReceiverById(this Web web, Guid id)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to process  

  

#### id  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;The id of event receiver  

  

### Return Value
Type: EventReceiverDefinition  
Returns an EventReceiverDefinition if succeeded. Returns null if failed.  


## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
