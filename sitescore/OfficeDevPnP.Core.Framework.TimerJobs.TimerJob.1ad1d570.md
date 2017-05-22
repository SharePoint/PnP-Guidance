# TimerJob.UpdateAddedSites Method  
 Virtual method that can be overriden to allow the timer job itself to control the list of sites to operate against. Scenario is for example timer job that reads this data from a database instead of being fed by the calling program   

**Namespace:** [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public virtual List<String> UpdateAddedSites(List<String> addedSites)
```
### Parameters
#### addedSites  
&emsp;&emsp;Type: System.Collections.Generic.List&lt;System.String&gt;  
&emsp;&emsp;List of added site Url's and/or wildcard site Url's  

  

### Return Value
Type: List<String>  
List of added site Url's and/or wildcard site Url's  


## See also
- [TimerJob](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.md) 
- [OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md) 
