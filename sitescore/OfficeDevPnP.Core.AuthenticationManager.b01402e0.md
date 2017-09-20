# AuthenticationManager.GetHighTrustCertificateAppOnlyAuthenticatedContext Method  
 Returns a SharePoint ClientContext using High Trust Certificate App Only Authentication   

**Namespace:** [OfficeDevPnP.Core](OfficeDevPnP.Core.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public ClientContext GetHighTrustCertificateAppOnlyAuthenticatedContext(String siteUrl, String clientId, String certificatePath, SecureString certificatePassword, String certificateIssuerId)
```
### Parameters
#### siteUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Site for which the ClientContext object will be instantiated  

  

#### clientId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The SharePoint Client ID  

  

#### certificatePath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Full path to the private key certificate (.pfx) used to authenticate  

  

#### certificatePassword  
&emsp;&emsp;Type: System.Security.SecureString  
&emsp;&emsp;Password used for the private key certificate (.pfx)  

  

#### certificateIssuerId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The IssuerID under which the CER counterpart of the PFX has been registered in SharePoint as a Trusted Security Token issuer  

  

### Return Value
Type: ClientContext  
Authenticated SharePoint ClientContext  


## See also
- [AuthenticationManager](OfficeDevPnP.Core.AuthenticationManager.md) 
- [OfficeDevPnP.Core](OfficeDevPnP.Core.md) 
