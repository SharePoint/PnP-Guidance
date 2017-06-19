# WorkflowExtensions.GetWorkflowDefinitions Method  
 Returns all the workflow definitions   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static WorkflowDefinition[] GetWorkflowDefinitions(this Web web, Boolean publishedOnly)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The target Web  

  

#### publishedOnly  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Defines whether to include only published definition, or all the definitions  

  

### Return Value
Type: WorkflowDefinition[]  
Returns all WorkflowDefinitions  


## See also
- [WorkflowExtensions](Microsoft.SharePoint.Client.WorkflowExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
