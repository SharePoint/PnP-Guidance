# AuthenticationManager.GetHighTrustCertificateAppOnlyAuthenticatedContext Method  
 Returns a SharePoint ClientContext using High Trust Certificate App Only Authentication   

**Namespace:** [OfficeDevPnP.Core](OfficeDevPnP.Core.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public ClientContext GetHighTrustCertificateAppOnlyAuthenticatedContext(String siteUrl, String clientId, X509Certificate2 certificate, String certificateIssuerId)
```
### Parameters
#### siteUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Site for which the ClientContext object will be instantiated  

  

#### clientId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The SharePoint Client ID  

  

#### certificate  
&emsp;&emsp;Type: System.Security.Cryptography.X509Certificates.X509Certificate2  
&emsp;&emsp;Private key certificate (.pfx) used to authenticate  

  

#### certificateIssuerId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The IssuerID under which the CER counterpart of the PFX has been registered in SharePoint as a Trusted Security Token issuer  

  

### Return Value
Type: ClientContext  
Authenticated SharePoint ClientContext  


## See also
- [AuthenticationManager](OfficeDevPnP.Core.AuthenticationManager.md) 
- [OfficeDevPnP.Core](OfficeDevPnP.Core.md) 
