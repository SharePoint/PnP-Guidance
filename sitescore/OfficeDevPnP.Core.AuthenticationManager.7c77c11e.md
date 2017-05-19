# AuthenticationManager.GetHighTrustCertificateAppOnlyAuthenticatedContext Method  
 Returns a SharePoint ClientContext using High Trust Certificate App Only Authentication   

**Namespace:** [OfficeDevPnP.Core](OfficeDevPnP.Core.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public ClientContext GetHighTrustCertificateAppOnlyAuthenticatedContext(String siteUrl, String clientId, StoreName storeName, StoreLocation storeLocation, String thumbPrint, String certificateIssuerId)
```
### Parameters
#### siteUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Site for which the ClientContext object will be instantiated  

  

#### clientId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The SharePoint Client ID  

  

#### storeName  
&emsp;&emsp;Type: System.Security.Cryptography.X509Certificates.StoreName  
&emsp;&emsp;The name of the store for the certificate  

  

#### storeLocation  
&emsp;&emsp;Type: System.Security.Cryptography.X509Certificates.StoreLocation  
&emsp;&emsp;The location of the store for the certificate  

  

#### thumbPrint  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The thumbprint of the certificate to locate in the store  

  

#### certificateIssuerId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The IssuerID under which the CER counterpart of the PFX has been registered in SharePoint as a Trusted Security Token issuer  

  

### Return Value
Type: ClientContext  
Authenticated SharePoint ClientContext  


## See also
- [AuthenticationManager](OfficeDevPnP.Core.AuthenticationManager.md) 
- [OfficeDevPnP.Core](OfficeDevPnP.Core.md) 
