# WebExtensions.AddRemoteEventReceiver Method  
 Registers a remote event receiver   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static EventReceiverDefinition AddRemoteEventReceiver(this Web web, String name, String url, EventReceiverType eventReceiverType, EventReceiverSynchronization synchronization, Int32 sequenceNumber, Boolean force)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The web to process  

  

#### name  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The name of the event receiver (needs to be unique among the event receivers registered on this list)  

  

#### url  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The URL of the remote WCF service that handles the event  

  

#### eventReceiverType  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.EventReceiverType  
&emsp;&emsp;The type of event for the event receiver.  

  

#### synchronization  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.EventReceiverSynchronization  
&emsp;&emsp;An enumeration that specifies the synchronization state for the event receiver.  

  

#### sequenceNumber  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;An integer that represents the relative sequence of the event.  

  

#### force  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;If True any event already registered with the same name will be removed first.  

  

### Return Value
Type: EventReceiverDefinition  
Returns an EventReceiverDefinition if succeeded. Returns null if failed.  


## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
