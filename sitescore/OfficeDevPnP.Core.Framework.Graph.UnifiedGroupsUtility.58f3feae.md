# UnifiedGroupsUtility.ListUnifiedGroups Method  
 Returns all the Office 365 Groups in the current Tenant based on a startIndex. IncludeSite adds additional properties about the Modern SharePoint Site backing the group   

**Namespace:** [OfficeDevPnP.Core.Framework.Graph](OfficeDevPnP.Core.Framework.Graph.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static List<UnifiedGroupEntity> ListUnifiedGroups(String accessToken, String displayName, String mailNickname, Int32 startIndex = 0, Int32 endIndex = 999, Boolean includeSite = True, Int32 retryCount = 10, Int32 delay = 500)
```
### Parameters
#### accessToken  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The OAuth 2.0 Access Token to use for invoking the Microsoft Graph  

  

#### (optional) displayName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The DisplayName of the Office 365 Group  

  

#### (optional) mailNickname  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The MailNickname of the Office 365 Group  

  

#### (optional) startIndex  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Not relevant anymore  

  

#### (optional) endIndex  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Not relevant anymore  

  

#### (optional) includeSite  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Defines whether to return details about the Modern SharePoint Site backing the group. Default is true.  

  

#### (optional) retryCount  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Number of times to retry the request in case of throttling  

  

#### (optional) delay  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Milliseconds to wait before retrying the request. The delay will be increased (doubled) every retry  

  

### Return Value
Type: List<UnifiedGroupEntity>  
An IList of SiteEntity objects  


## See also
- [UnifiedGroupsUtility](OfficeDevPnP.Core.Framework.Graph.UnifiedGroupsUtility.md) 
- [OfficeDevPnP.Core.Framework.Graph](OfficeDevPnP.Core.Framework.Graph.md) 
