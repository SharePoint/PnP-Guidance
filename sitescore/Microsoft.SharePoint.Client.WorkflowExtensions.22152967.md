# WorkflowExtensions.AddWorkflowSubscription Method  
 Adds a workflow subscription to a list   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Guid AddWorkflowSubscription(this List list, WorkflowDefinition workflowDefinition, String subscriptionName, Boolean startManually, Boolean startOnCreate, Boolean startOnChange, String historyListName, String taskListName, Dictionary<String, String> associationValues)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;The target list  

  

#### workflowDefinition  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.WorkflowServices.WorkflowDefinition  
&emsp;&emsp;The workflow definition. WorkflowExtensions.GetWorkflowDefinition  

  

#### subscriptionName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The name of the workflow subscription to create  

  

#### startManually  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;if True the workflow can be started manually  

  

#### startOnCreate  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;if True the workflow will be started on item creation  

  

#### startOnChange  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;if True the workflow will be started on item change  

  

#### historyListName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;the name of the history list. If not available it will be created  

  

#### taskListName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;the name of the task list. If not available it will be created  

  

#### (optional) associationValues  
&emsp;&emsp;Type: System.Collections.Generic.Dictionary&lt;System.String, System.String&gt;  
&emsp;&emsp;the name-value pairs for workflow definition  

  

### Return Value
Type: Guid  
Guid of the workflow subscription  


## See also
- [WorkflowExtensions](Microsoft.SharePoint.Client.WorkflowExtensions.md) 
- [GetWorkflowDefinition](Microsoft.SharePoint.Client.WorkflowExtensions.89d3977b.md)
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
