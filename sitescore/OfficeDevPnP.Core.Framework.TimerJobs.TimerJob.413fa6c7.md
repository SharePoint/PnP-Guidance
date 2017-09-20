# TimerJob.UseNetworkCredentialsAuthentication Method  
 Prepares the timerjob to operate against SharePoint on-premises with user name password credentials which are retrieved via the windows Credential Manager. Sets AuthenticationType to AuthenticationType.NetworkCredentials   

**Namespace:** [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public void UseNetworkCredentialsAuthentication(String credentialName)
```
### Parameters
#### credentialName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the credential manager registration  

  

### Return Value
Type: void  

## See also
- [TimerJob](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.md) 
- [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md) 
