# AuthenticationManager.RefreshADFSCertificateMixedAuthenticationContext Method  
 Refreshes the SharePoint FedAuth cookie   

**Namespace:** [OfficeDevPnP.Core](OfficeDevPnP.Core.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public void RefreshADFSCertificateMixedAuthenticationContext(String siteUrl, String serialNumber, String sts, String idpId, Int32 logonTokenCacheExpirationWindow = 10)
```
### Parameters
#### siteUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Url of the SharePoint site that's secured via ADFS  

  

#### serialNumber  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Represents the serial number of the certificate as displayed by the certificate dialog box, but without the spaces, or as returned by the System.Security.Cryptography.X509Certificates.X509Certificate.GetSerialNumberString method  

  

#### sts  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Hostname of the ADFS server (e.g. sts.company.com)  

  

#### idpId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Identifier of the ADFS relying party that we're hitting  

  

#### (optional) logonTokenCacheExpirationWindow  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Optioanlly provide the value of the SharePoint STS logonTokenCacheExpirationWindow. Defaults to 10 minutes.  

  

### Return Value
Type: void  
ClientContext to be used by CSOM code  


## See also
- [AuthenticationManager](OfficeDevPnP.Core.AuthenticationManager.md) 
- [OfficeDevPnP.Core](OfficeDevPnP.Core.md) 
