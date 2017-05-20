# ListExtensions.AddRemoteEventReceiver Method  
 Registers a remote event receiver   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static EventReceiverDefinition AddRemoteEventReceiver(this List list, String name, String url, EventReceiverType eventReceiverType, EventReceiverSynchronization synchronization, Boolean force)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;The list to process  

  

#### name  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The name of the event receiver (needs to be unique among the event receivers registered on this list)  

  

#### url  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The URL of the remote WCF service that handles the event  

  

#### eventReceiverType  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.EventReceiverType  
&emsp;&emsp; Registers a remote event receiver   

  

#### synchronization  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.EventReceiverSynchronization  
&emsp;&emsp; Registers a remote event receiver   

  

#### force  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;If True any event already registered with the same name will be removed first.  

  

### Return Value
Type: EventReceiverDefinition  
Returns an EventReceiverDefinition if succeeded. Returns null if failed.  


## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
