# TimerJob.UseAzureADAppOnlyAuthentication Method  
 Prepares the timerjob to operate against SharePoint Only with Azure AD app-only credentials. Sets AuthenticationType to AuthenticationType.AzureADAppOnly   

**Namespace:** [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public void UseAzureADAppOnlyAuthentication(String clientId, String azureTenant, X509Certificate2 certificate)
```
### Parameters
#### clientId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Client ID of the app  

  

#### azureTenant  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The Azure tenant name, like contoso.com  

  

#### certificate  
&emsp;&emsp;Type: System.Security.Cryptography.X509Certificates.X509Certificate2  
&emsp;&emsp;The X.509 Certificate to use for AppOnly Authentication  

  

### Return Value
Type: void  

## See also
- [TimerJob](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.md) 
- [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md) 
