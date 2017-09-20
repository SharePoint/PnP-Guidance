# TimerJob.UseAzureADAppOnlyAuthentication Method  
 Prepares the timerjob to operate against SharePoint Only with Azure AD app-only credentials. Sets AuthenticationType to AuthenticationType.AzureADAppOnly   

**Namespace:** [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public void UseAzureADAppOnlyAuthentication(String clientId, String azureTenant, String certificatePath, String certificatePassword)
```
### Parameters
#### clientId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Client ID of the app  

  

#### azureTenant  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The Azure tenant name, like contoso.com  

  

#### certificatePath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The path to the *.pfx certicate file  

  

#### certificatePassword  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The password to the certificate  

  

### Return Value
Type: void  

## See also
- [TimerJob](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.md) 
- [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md) 
