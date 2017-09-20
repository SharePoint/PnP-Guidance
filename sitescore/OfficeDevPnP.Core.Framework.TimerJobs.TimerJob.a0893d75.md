# TimerJob.UseOffice365Authentication Method  
 Prepares the timerjob to operate against Office 365 with user and password credentials. Sets AuthenticationType to AuthenticationType.Office365   

**Namespace:** [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public void UseOffice365Authentication(String userUPN, SecureString password)
```
### Parameters
#### userUPN  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;user name  

  

#### password  
&emsp;&emsp;Type: System.Security.SecureString  
&emsp;&emsp;Password of the user that will be used to operate the timer job work  

  

### Return Value
Type: void  

## See also
- [TimerJob](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.md) 
- [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md) 
