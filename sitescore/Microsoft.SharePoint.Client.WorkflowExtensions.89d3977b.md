# WorkflowExtensions.GetWorkflowDefinition Method  
 Returns a workflow definition for a site   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static WorkflowDefinition GetWorkflowDefinition(this Web web, String displayName, Boolean publishedOnly = True)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;the target web  

  

#### displayName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;the workflow definition display name, which is displayed to users  

  

#### (optional) publishedOnly  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Defines whether to include only published definition, or all the definitions  

  

### Return Value
Type: WorkflowDefinition  
Returns a WorkflowDefinition object  


## See also
- [WorkflowExtensions](Microsoft.SharePoint.Client.WorkflowExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
