# TimerJob.Clone Method  
 Takes over the settings from the passed timer job. Is useful when you run multiple jobs in a row or chain job execution. Settings that are taken over are all the authentication, enumeration settings and SharePointVersion   

**Namespace:** [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public void Clone(TimerJob job)
```
### Parameters
#### job  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.TimerJobs.TimerJob](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.md)  
&emsp;&emsp;TimerJob  

  

### Return Value
Type: void  

## See also
- [TimerJob](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.md) 
- [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md) 
