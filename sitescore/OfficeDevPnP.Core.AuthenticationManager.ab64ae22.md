# AuthenticationManager.GetAzureADAppOnlyAuthenticatedContext Method  
 Returns a SharePoint ClientContext using Azure Active Directory App Only Authentication. This requires that you have a certificated created, and updated the key credentials key in the application manifest in the azure AD accordingly.   

**Namespace:** [OfficeDevPnP.Core](OfficeDevPnP.Core.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public ClientContext GetAzureADAppOnlyAuthenticatedContext(String siteUrl, String clientId, String tenant, X509Certificate2 certificate, AzureEnvironment environment = 0)
```
### Parameters
#### siteUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Site for which the ClientContext object will be instantiated  

  

#### clientId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The Azure AD Application Client ID  

  

#### tenant  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The Azure AD Tenant, e.g. mycompany.onmicrosoft.com  

  

#### certificate  
&emsp;&emsp;Type: System.Security.Cryptography.X509Certificates.X509Certificate2  
&emsp;&emsp;Certificate used to authenticate  

  

#### (optional) environment  
&emsp;&emsp;Type: [OfficeDevPnP.Core.AzureEnvironment](OfficeDevPnP.Core.AzureEnvironment.md)  
&emsp;&emsp;SharePoint environment being used  

  

### Return Value
Type: ClientContext  
  


## See also
- [AuthenticationManager](OfficeDevPnP.Core.AuthenticationManager.md) 
- [OfficeDevPnP.Core](OfficeDevPnP.Core.md) 
