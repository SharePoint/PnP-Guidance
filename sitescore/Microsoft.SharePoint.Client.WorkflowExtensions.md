# WorkflowExtensions Class
 Class for deprecated workflow extension methods   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class WorkflowExtensions
```
## Extension Methods
|**Name**|**Description**|
|:-----|:-----|
| [AddWorkflowDefinition(Web, WorkflowDefinition, Boolean)](Microsoft.SharePoint.Client.WorkflowExtensions.ed3d4bd4.md) | Adds a workflow definition
| [AddWorkflowSubscription(List, String, String, Boolean, Boolean, Boolean, String, String, Dictionary&lt;String, String&gt;)](Microsoft.SharePoint.Client.WorkflowExtensions.db48bc3.md) | Adds a workflow subscription
| [AddWorkflowSubscription(List, WorkflowDefinition, String, Boolean, Boolean, Boolean, String, String, Dictionary&lt;String, String&gt;)](Microsoft.SharePoint.Client.WorkflowExtensions.22152967.md) | Adds a workflow subscription to a list
| [CancelWorkFlow(WorkflowInstance)](Microsoft.SharePoint.Client.WorkflowExtensions.1afb83c2.md) | Cancels a workflow instance
| [Delete(WorkflowSubscription)](Microsoft.SharePoint.Client.WorkflowExtensions.7b09533.md) | Deletes the subscription
| [Delete(WorkflowDefinition)](Microsoft.SharePoint.Client.WorkflowExtensions.fa0bc740.md) | Deletes a workflow definition
| [GetInstances(WorkflowSubscription)](Microsoft.SharePoint.Client.WorkflowExtensions.41117fbe.md) | Returns all instances of a workflow for this subscription
| [GetWorkflowDefinition(Web, String, Boolean)](Microsoft.SharePoint.Client.WorkflowExtensions.89d3977b.md) | Returns a workflow definition for a site
| [GetWorkflowDefinition(Web, Guid)](Microsoft.SharePoint.Client.WorkflowExtensions.1a9b07c5.md) | Returns a workflow definition
| [GetWorkflowDefinitions(Web, Boolean)](Microsoft.SharePoint.Client.WorkflowExtensions.7692b016.md) | Returns all the workflow definitions
| [GetWorkflowInstances(Web)](Microsoft.SharePoint.Client.WorkflowExtensions.57799136.md) | Returns alls workflow instances for a site
| [GetWorkflowInstances(Web, ListItem)](Microsoft.SharePoint.Client.WorkflowExtensions.d66b2fcc.md) | Returns alls workflow instances for a list item
| [GetWorkflowSubscription(Web, String)](Microsoft.SharePoint.Client.WorkflowExtensions.250dcc40.md) | Returns a workflow subscription for a site.
| [GetWorkflowSubscription(Web, Guid)](Microsoft.SharePoint.Client.WorkflowExtensions.cd867166.md) | Returns a workflow subscription
| [GetWorkflowSubscription(List, String)](Microsoft.SharePoint.Client.WorkflowExtensions.7fa8d0c5.md) | Returns a workflow subscription (associations) for a list
| [GetWorkflowSubscriptions(Web)](Microsoft.SharePoint.Client.WorkflowExtensions.74365dec.md) | Returns all the workflow subscriptions (associations) for the web and the lists of that web
| [PublishCustomEvent(WorkflowInstance, String, String)](Microsoft.SharePoint.Client.WorkflowExtensions.41011483.md) | Publish a custom event to a target workflow instance
| [ResumeWorkflow(WorkflowInstance)](Microsoft.SharePoint.Client.WorkflowExtensions.64c0f0e1.md) | Resumes a workflow
| [StartWorkflowInstance(Web, String, IDictionary&lt;String, Object&gt;)](Microsoft.SharePoint.Client.WorkflowExtensions.1af92fba.md) | Starts a new instance of a workflow definition against the current web site
| [StartWorkflowInstance(Web, Guid, IDictionary&lt;String, Object&gt;)](Microsoft.SharePoint.Client.WorkflowExtensions.f1316769.md) | Starts a new instance of a workflow definition against the current web site
| [StartWorkflowInstance(ListItem, String, IDictionary&lt;String, Object&gt;)](Microsoft.SharePoint.Client.WorkflowExtensions.b77b236e.md) | Starts a new instance of a workflow definition against the current item
| [StartWorkflowInstance(ListItem, Guid, IDictionary&lt;String, Object&gt;)](Microsoft.SharePoint.Client.WorkflowExtensions.f71820e3.md) | Starts a new instance of a workflow definition against the current item
## See also
- WorkflowExtensions.GetWorkflowDefinition
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)
