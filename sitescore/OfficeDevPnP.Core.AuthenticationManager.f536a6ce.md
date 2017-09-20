# AuthenticationManager.GetAzureADNativeApplicationAuthenticatedContext Method  
 Returns a SharePoint ClientContext using Azure Active Directory authentication. This requires that you have a Azure AD Native Application registered. The user will be prompted for authentication.   

**Namespace:** [OfficeDevPnP.Core](OfficeDevPnP.Core.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public ClientContext GetAzureADNativeApplicationAuthenticatedContext(String siteUrl, String clientId, Uri redirectUri, TokenCache tokenCache, AzureEnvironment environment = 0)
```
### Parameters
#### siteUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Site for which the ClientContext object will be instantiated  

  

#### clientId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The Azure AD Native Application Client ID  

  

#### redirectUri  
&emsp;&emsp;Type: System.Uri  
&emsp;&emsp;The Azure AD Native Application Redirect Uri  

  

#### (optional) tokenCache  
&emsp;&emsp;Type: Microsoft.IdentityModel.Clients.ActiveDirectory.TokenCache  
&emsp;&emsp;Optional token cache. If not specified an in-memory token cache will be used  

  

#### (optional) environment  
&emsp;&emsp;Type: [OfficeDevPnP.Core.AzureEnvironment](OfficeDevPnP.Core.AzureEnvironment.md)  
&emsp;&emsp;SharePoint environment being used  

  

### Return Value
Type: ClientContext  
Client context object  


## See also
- [AuthenticationManager](OfficeDevPnP.Core.AuthenticationManager.md) 
- [OfficeDevPnP.Core](OfficeDevPnP.Core.md) 
