# UnifiedGroupsUtility.GetUnifiedGroup Method  
 Get an Office 365 Group (i.e. Unified Group) by Id   

**Namespace:** [OfficeDevPnP.Core.Framework.Graph](OfficeDevPnP.Core.Framework.Graph.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static UnifiedGroupEntity GetUnifiedGroup(String groupId, String accessToken, Int32 retryCount = 10, Int32 delay = 500, Boolean includeSite = True)
```
### Parameters
#### groupId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The ID of the Office 365 Group  

  

#### accessToken  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The OAuth 2.0 Access Token to use for invoking the Microsoft Graph  

  

#### (optional) retryCount  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Number of times to retry the request in case of throttling  

  

#### (optional) delay  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Milliseconds to wait before retrying the request. The delay will be increased (doubled) every retry  

  

#### (optional) includeSite  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Defines whether to return details about the Modern SharePoint Site backing the group. Default is true.  

  

### Return Value
Type: [UnifiedGroupEntity](OfficeDevPnP.Core.Entities.UnifiedGroupEntity.md)  

## See also
- [UnifiedGroupsUtility](OfficeDevPnP.Core.Framework.Graph.UnifiedGroupsUtility.md) 
- [OfficeDevPnP.Core.Framework.Graph](OfficeDevPnP.Core.Framework.Graph.md) 
