# X509CertificateUtility.Encrypt Method  
 Encrypts data based on the RSACryptoServiceProvider   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Byte[] Encrypt(Byte[] plainData, Boolean fOAEP, X509Certificate2 certificate)
```
### Parameters
#### plainData  
&emsp;&emsp;Type: System.Byte[]  
&emsp;&emsp;Bytes to encrypt  

  

#### fOAEP  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp; true to perform direct System.Security.Cryptography.RSA decryption using OAEP padding  

  

#### certificate  
&emsp;&emsp;Type: System.Security.Cryptography.X509Certificates.X509Certificate2  
&emsp;&emsp;Certificate to use  

  

### Return Value
Type: Byte[]  
Encrypted bytes  


## See also
- [X509CertificateUtility](OfficeDevPnP.Core.Utilities.X509CertificateUtility.md) 
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md) 
