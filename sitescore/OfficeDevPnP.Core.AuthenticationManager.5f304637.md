# AuthenticationManager.GetAzureADWebApplicationAuthenticatedContext Method  
 Returns a SharePoint ClientContext using Azure Active Directory authentication. This requires that you have a Azure AD Web Application registered. The user will not be prompted for authentication, the current user's authentication context will be used by leveraging ADAL.   

**Namespace:** [OfficeDevPnP.Core](OfficeDevPnP.Core.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public ClientContext GetAzureADWebApplicationAuthenticatedContext(String siteUrl, Func<String, String> accessTokenGetter)
```
### Parameters
#### siteUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Site for which the ClientContext object will be instantiated  

  

#### accessTokenGetter  
&emsp;&emsp;Type: System.Func&lt;System.String, System.String&gt;  
&emsp;&emsp;The AccessToken getter method to use  

  

### Return Value
Type: ClientContext  
Client context object  


## See also
- [AuthenticationManager](OfficeDevPnP.Core.AuthenticationManager.md) 
- [OfficeDevPnP.Core](OfficeDevPnP.Core.md) 
