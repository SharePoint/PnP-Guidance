# UnifiedGroupsUtility.UpdateUnifiedGroup Method  
 Updates the logo, members or visibility state of an Office 365 Group   

**Namespace:** [OfficeDevPnP.Core.Framework.Graph](OfficeDevPnP.Core.Framework.Graph.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool UpdateUnifiedGroup(String groupId, String accessToken, Int32 retryCount = 10, Int32 delay = 500, String displayName, String description, String[] owners, String[] members, Stream groupLogo, Boolean isPrivate = False)
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

  

#### (optional) displayName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The Display Name for the Office 365 Group  

  

#### (optional) description  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The Description for the Office 365 Group  

  

#### (optional) owners  
&emsp;&emsp;Type: System.String[]  
&emsp;&emsp;A list of UPNs for group owners, if any, to be added to the site  

  

#### (optional) members  
&emsp;&emsp;Type: System.String[]  
&emsp;&emsp;A list of UPNs for group members, if any, to be added to the site  

  

#### (optional) groupLogo  
&emsp;&emsp;Type: System.IO.Stream  
&emsp;&emsp;The binary stream of the logo for the Office 365 Group  

  

#### (optional) isPrivate  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Defines whether the group will be private or public, optional with default false (i.e. public)  

  

### Return Value
Type: bool  
Declares whether the Office 365 Group has been updated or not  


## See also
- [UnifiedGroupsUtility](OfficeDevPnP.Core.Framework.Graph.UnifiedGroupsUtility.md) 
- [OfficeDevPnP.Core.Framework.Graph](OfficeDevPnP.Core.Framework.Graph.md) 
