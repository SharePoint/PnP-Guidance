# TimerJob.UseNetworkCredentialsAuthentication Method  
 Prepares the timerjob to operate against SharePoint on-premises with user name password credentials. Sets AuthenticationType to AuthenticationType.NetworkCredentials   

**Namespace:** [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public void UseNetworkCredentialsAuthentication(String samAccountName, String password, String domain)
```
### Parameters
#### samAccountName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;samAccontName of the windows user  

  

#### password  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Password of the windows user  

  

#### domain  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;NT domain of the windows user  

  

### Return Value
Type: void  

## See also
- [TimerJob](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.md) 
- [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md) 
