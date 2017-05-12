# AuthenticationManager Class
 This manager class can be used to obtain a SharePointContext object   

**Namespace:** [OfficeDevPnP.Core](OfficeDevPnP.Core.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public class AuthenticationManager
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [AuthenticationManager()](OfficeDevPnP.Core.AuthenticationManager.ctor1.md) |  This manager class can be used to obtain a SharePointContext object 
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [GetADFSCertificateMixedAuthenticationContext(String, String, String, String, Int32)](OfficeDevPnP.Core.AuthenticationManager.59da3ba5.md) | Returns a SharePoint on-premises ClientContext for sites secured via ADFS
| [GetADFSUserNameMixedAuthenticatedContext(String, String, String, String, String, String, Int32)](OfficeDevPnP.Core.AuthenticationManager.375fa96b.md) | Returns a SharePoint on-premises ClientContext for sites secured via ADFS
| [GetAppOnlyAuthenticatedContext(String, String, String)](OfficeDevPnP.Core.AuthenticationManager.d811a03e.md) | Returns an app only ClientContext object
| [GetAppOnlyAuthenticatedContext(String, String, String, AzureEnvironment)](OfficeDevPnP.Core.AuthenticationManager.58eb50ac.md) | Returns an app only ClientContext object
| [GetAppOnlyAuthenticatedContext(String, String, String, String, String, String)](OfficeDevPnP.Core.AuthenticationManager.72a4a663.md) | Returns an app only ClientContext object
| [GetAzureADAccessTokenAuthenticatedContext(String, String)](OfficeDevPnP.Core.AuthenticationManager.16efabf6.md) | Returns a SharePoint ClientContext using Azure Active Directory authentication. This requires that you have a Azure AD Web Application registered. The user will not be prompted for authentication, the current user's authentication context will be used by leveraging an explicit OAuth 2.0 Access Token value.
| [GetAzureADACSEndPoint(AzureEnvironment)](OfficeDevPnP.Core.AuthenticationManager.6f718dbe.md) | Get's the Azure ASC login end point for the given environment
| [GetAzureADACSEndPointPrefix(AzureEnvironment)](OfficeDevPnP.Core.AuthenticationManager.7b94031f.md) | Get's the Azure ACS login end point prefix for the given environment
| [GetAzureADAppOnlyAuthenticatedContext(String, String, String, StoreName, StoreLocation, String, AzureEnvironment)](OfficeDevPnP.Core.AuthenticationManager.9589d33.md) | Returns a SharePoint ClientContext using Azure Active Directory App Only Authentication. This requires that you have a certificated created, and updated the key credentials key in the application manifest in the azure AD accordingly.
| [GetAzureADAppOnlyAuthenticatedContext(String, String, String, String, String, AzureEnvironment)](OfficeDevPnP.Core.AuthenticationManager.bb8969a5.md) | Returns a SharePoint ClientContext using Azure Active Directory App Only Authentication. This requires that you have a certificated created, and updated the key credentials key in the application manifest in the azure AD accordingly.
| [GetAzureADAppOnlyAuthenticatedContext(String, String, String, String, SecureString, AzureEnvironment)](OfficeDevPnP.Core.AuthenticationManager.67fba39e.md) | Returns a SharePoint ClientContext using Azure Active Directory App Only Authentication. This requires that you have a certificated created, and updated the key credentials key in the application manifest in the azure AD accordingly.
| [GetAzureADAppOnlyAuthenticatedContext(String, String, String, X509Certificate2, AzureEnvironment)](OfficeDevPnP.Core.AuthenticationManager.ab64ae22.md) | Returns a SharePoint ClientContext using Azure Active Directory App Only Authentication. This requires that you have a certificated created, and updated the key credentials key in the application manifest in the azure AD accordingly.
| [GetAzureADLoginEndPoint(AzureEnvironment)](OfficeDevPnP.Core.AuthenticationManager.13a3dc47.md) | Get's the Azure AD login end point for the given environment
| [GetAzureADNativeApplicationAuthenticatedContext(String, String, String, TokenCache, AzureEnvironment)](OfficeDevPnP.Core.AuthenticationManager.4f3ffdaa.md) | Returns a SharePoint ClientContext using Azure Active Directory authentication. This requires that you have a Azure AD Native Application registered. The user will be prompted for authentication.
| [GetAzureADNativeApplicationAuthenticatedContext(String, String, Uri, TokenCache, AzureEnvironment)](OfficeDevPnP.Core.AuthenticationManager.f536a6ce.md) | Returns a SharePoint ClientContext using Azure Active Directory authentication. This requires that you have a Azure AD Native Application registered. The user will be prompted for authentication.
| [GetAzureADWebApplicationAuthenticatedContext(String, Func&lt;String, String&gt;)](OfficeDevPnP.Core.AuthenticationManager.5f304637.md) | Returns a SharePoint ClientContext using Azure Active Directory authentication. This requires that you have a Azure AD Web Application registered. The user will not be prompted for authentication, the current user's authentication context will be used by leveraging ADAL.
| [GetHighTrustCertificateAppOnlyAuthenticatedContext(String, String, String, String, String)](OfficeDevPnP.Core.AuthenticationManager.150f5e59.md) | Returns a SharePoint ClientContext using High Trust Certificate App Only Authentication
| [GetHighTrustCertificateAppOnlyAuthenticatedContext(String, String, String, SecureString, String)](OfficeDevPnP.Core.AuthenticationManager.b01402e0.md) | Returns a SharePoint ClientContext using High Trust Certificate App Only Authentication
| [GetHighTrustCertificateAppOnlyAuthenticatedContext(String, String, StoreName, StoreLocation, String, String)](OfficeDevPnP.Core.AuthenticationManager.7c77c11e.md) | Returns a SharePoint ClientContext using High Trust Certificate App Only Authentication
| [GetHighTrustCertificateAppOnlyAuthenticatedContext(String, String, X509Certificate2, String)](OfficeDevPnP.Core.AuthenticationManager.9cfa9c25.md) | Returns a SharePoint ClientContext using High Trust Certificate App Only Authentication
| [GetNetworkCredentialAuthenticatedContext(String, String, String, String)](OfficeDevPnP.Core.AuthenticationManager.d3aeb52f.md) | Returns a SharePoint on-premises / SharePoint Online Dedicated ClientContext object
| [GetNetworkCredentialAuthenticatedContext(String, String, SecureString, String)](OfficeDevPnP.Core.AuthenticationManager.34c7cc73.md) | Returns a SharePoint on-premises / SharePoint Online Dedicated ClientContext object
| [GetSharePointOnlineAuthenticatedContextTenant(String, String, String)](OfficeDevPnP.Core.AuthenticationManager.e8fa5bc2.md) | Returns a SharePointOnline ClientContext object
| [GetSharePointOnlineAuthenticatedContextTenant(String, String, SecureString)](OfficeDevPnP.Core.AuthenticationManager.25cc8181.md) | Returns a SharePointOnline ClientContext object
| [GetWebLoginClientContext(String, Icon)](OfficeDevPnP.Core.AuthenticationManager.99809936.md) | Returns a SharePoint on-premises / SharePoint Online ClientContext object. Requires claims based authentication with FedAuth cookie.
| [RefreshADFSCertificateMixedAuthenticationContext(String, String, String, String, Int32)](OfficeDevPnP.Core.AuthenticationManager.ed20f39f.md) | Refreshes the SharePoint FedAuth cookie
| [RefreshADFSUserNameMixedAuthenticatedContext(String, String, String, String, String, String, Int32)](OfficeDevPnP.Core.AuthenticationManager.23b7c2d8.md) | Refreshes the SharePoint FedAuth cookie
## See also
- [OfficeDevPnP.Core](OfficeDevPnP.Core.md)
