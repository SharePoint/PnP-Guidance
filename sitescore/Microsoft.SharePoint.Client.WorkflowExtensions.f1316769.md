# WorkflowExtensions.StartWorkflowInstance Method  
 Starts a new instance of a workflow definition against the current web site   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Guid StartWorkflowInstance(this Web web, Guid subscriptionId, IDictionary<String, Object> payload)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The target web site  

  

#### subscriptionId  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;The ID of the workflow subscription to start  

  

#### payload  
&emsp;&emsp;Type: System.Collections.Generic.IDictionary&lt;System.String, System.Object&gt;  
&emsp;&emsp;Any input argument for the workflow instance  

  

### Return Value
Type: Guid  
The ID of the just started workflow instance  


## See also
- [WorkflowExtensions](Microsoft.SharePoint.Client.WorkflowExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
