# X509CertificateUtility.LoadCertificate Method  
 Loads a certificate from a given certificate store   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static X509Certificate2 LoadCertificate(StoreName storeName, StoreLocation storeLocation, String thumbprint)
```
### Parameters
#### storeName  
&emsp;&emsp;Type: System.Security.Cryptography.X509Certificates.StoreName  
&emsp;&emsp;Name of the certificate store  

  

#### storeLocation  
&emsp;&emsp;Type: System.Security.Cryptography.X509Certificates.StoreLocation  
&emsp;&emsp;Location of the certificate store  

  

#### thumbprint  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Thumbprint of the certificate to load  

  

### Return Value
Type: X509Certificate2  
An System.Security.Cryptography.X509Certificates.X509Certificate2 certificate  


## See also
- [X509CertificateUtility](OfficeDevPnP.Core.Utilities.X509CertificateUtility.md) 
- System.Security.Cryptography.X509Certificates.X509Certificate2
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md) 
