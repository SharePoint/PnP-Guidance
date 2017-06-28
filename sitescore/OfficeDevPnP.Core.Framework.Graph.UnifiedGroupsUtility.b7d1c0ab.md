# UnifiedGroupsUtility.CreateUnifiedGroup Method  
 Creates a new Office 365 Group (i.e. Unified Group) with its backing Modern SharePoint Site   

**Namespace:** [OfficeDevPnP.Core.Framework.Graph](OfficeDevPnP.Core.Framework.Graph.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static UnifiedGroupEntity CreateUnifiedGroup(String displayName, String description, String mailNickname, String accessToken, String[] owners, String[] members, Stream groupLogo, Boolean isPrivate = False, Int32 retryCount = 10, Int32 delay = 500)
```
### Parameters
#### displayName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The Display Name for the Office 365 Group  

  

#### description  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The Description for the Office 365 Group  

  

#### mailNickname  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The Mail Nickname for the Office 365 Group  

  

#### accessToken  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The OAuth 2.0 Access Token to use for invoking the Microsoft Graph  

  

#### (optional) owners  
&emsp;&emsp;Type: System.String[]  
&emsp;&emsp;A list of UPNs for group owners, if any  

  

#### (optional) members  
&emsp;&emsp;Type: System.String[]  
&emsp;&emsp;A list of UPNs for group members, if any  

  

#### (optional) groupLogo  
&emsp;&emsp;Type: System.IO.Stream  
&emsp;&emsp;The binary stream of the logo for the Office 365 Group  

  

#### (optional) isPrivate  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Defines whether the group will be private or public, optional with default false (i.e. public)  

  

#### (optional) retryCount  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Number of times to retry the request in case of throttling  

  

#### (optional) delay  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Milliseconds to wait before retrying the request. The delay will be increased (doubled) every retry  

  

### Return Value
Type: [UnifiedGroupEntity](OfficeDevPnP.Core.Entities.UnifiedGroupEntity.md)  
The just created Office 365 Group  


## See also
- [UnifiedGroupsUtility](OfficeDevPnP.Core.Framework.Graph.UnifiedGroupsUtility.md) 
- [OfficeDevPnP.Core.Framework.Graph](OfficeDevPnP.Core.Framework.Graph.md) 
