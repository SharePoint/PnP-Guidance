# WorkflowSubscription Class
 Defines a Workflow Subscription to provision   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel](OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel.md)  
## Syntax
```C#
public class WorkflowSubscription: BaseModel, IEquatable<WorkflowSubscription>
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [WorkflowSubscription()](OfficeDevPnP.Core.Framework.Provisioning.Model.WorkflowSubscription.ctor1.md) | Default Constructor 
| [WorkflowSubscription(Dictionary<String, String>)](OfficeDevPnP.Core.Framework.Provisioning.Model.WorkflowSubscription.ctor2.md) | Constructor 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [DefinitionId](OfficeDevPnP.Core.Framework.Provisioning.Model.WorkflowSubscription.DefinitionId.md) | Defines the ID of the Workflow Definition for the current Subscription
| [Enabled](OfficeDevPnP.Core.Framework.Provisioning.Model.WorkflowSubscription.Enabled.md) | Defines if the Workflow Definition is enabled for the current Subscription
| [EventSourceId](OfficeDevPnP.Core.Framework.Provisioning.Model.WorkflowSubscription.EventSourceId.md) | Defines the ID of the Event Source for the current Subscription
| [EventTypes](OfficeDevPnP.Core.Framework.Provisioning.Model.WorkflowSubscription.EventTypes.md) | Defines the list of events that will start the workflow instance
| [ListId](OfficeDevPnP.Core.Framework.Provisioning.Model.WorkflowSubscription.ListId.md) | Defines the ID of the target list/library for the current Subscription,
| [ManualStartBypassesActivationLimit](OfficeDevPnP.Core.Framework.Provisioning.Model.WorkflowSubscription.ManualStartBypassesActivationLimit.md) | Defines if the Workflow can be manually started bypassing the activation limit
| [Name](OfficeDevPnP.Core.Framework.Provisioning.Model.WorkflowSubscription.Name.md) | Defines the Name of the Workflow Subscription
| [ParentContentTypeId](OfficeDevPnP.Core.Framework.Provisioning.Model.WorkflowSubscription.ParentContentTypeId.md) | Defines the Parent ContentType Id of the Workflow Subscription
| [PropertyDefinitions](OfficeDevPnP.Core.Framework.Provisioning.Model.WorkflowSubscription.PropertyDefinitions.md) | Defines the Property Definitions of the Workflows to provision
| [StatusFieldName](OfficeDevPnP.Core.Framework.Provisioning.Model.WorkflowSubscription.StatusFieldName.md) | Defines the Status Field Name of the Workflow Subscription
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Equals(Object)](OfficeDevPnP.Core.Framework.Provisioning.Model.WorkflowSubscription.3520ddbb.md) | Comapres given workflow subscription object which is to be provisioned
| [Equals(WorkflowSubscription)](OfficeDevPnP.Core.Framework.Provisioning.Model.WorkflowSubscription.ed86df1.md) | Comapres given workflow subscription object which is to be provisioned
| [GetHashCode()](OfficeDevPnP.Core.Framework.Provisioning.Model.WorkflowSubscription.1c6872bd.md) | Gets hash code of workflow subscription
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
