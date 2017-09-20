# WorkflowExtensions.AddWorkflowDefinition Method  
 Adds a workflow definition   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Guid AddWorkflowDefinition(this Web web, WorkflowDefinition definition, Boolean publish = True)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;the target web  

  

#### definition  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.WorkflowServices.WorkflowDefinition  
&emsp;&emsp;the workflow definition to add  

  

#### (optional) publish  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;specify true to publish workflow definition  

  

### Return Value
Type: Guid  
  


## See also
- [WorkflowExtensions](Microsoft.SharePoint.Client.WorkflowExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
