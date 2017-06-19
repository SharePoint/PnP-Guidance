# WorkflowExtensions.PublishCustomEvent Method  
 Publish a custom event to a target workflow instance   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void PublishCustomEvent(this WorkflowInstance instance, String eventName, String payload)
```
### Parameters
#### instance  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.WorkflowServices.WorkflowInstance  
&emsp;&emsp;the workflow instance to publish event  

  

#### eventName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The name of the target event  

  

#### payload  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The payload that will be sent to the event  

  

### Return Value
Type: void  

## See also
- [WorkflowExtensions](Microsoft.SharePoint.Client.WorkflowExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
