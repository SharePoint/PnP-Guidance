# TimerJob.SetEnumerationCredentials Method  
 Provides the timer job with the enumeration credentials. For SharePoint on-premises username, password and domain are needed   

**Namespace:** [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public void SetEnumerationCredentials(String samAccountName, SecureString password, String domain)
```
### Parameters
#### samAccountName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Account name of the enumeration user  

  

#### password  
&emsp;&emsp;Type: System.Security.SecureString  
&emsp;&emsp;Password of the enumeration user  

  

#### domain  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Domain of the enumeration user  

  

### Return Value
Type: void  

## See also
- [TimerJob](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.md) 
- [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md) 
