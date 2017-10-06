# PnPHttpProvider.PnPHttpProvider members 
 Constructor with HttpMessageHandler   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public PnPHttpProvider(HttpMessageHandler innerHandler, int retryCount, int delay, string userAgent)
```
### Parameters
#### innerHandler  
&emsp;&emsp;Type: System.Net.Http.HttpMessageHandler  
&emsp;&emsp;HttpMessageHandler instance to pass along  


#### (optional) retryCount  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Number of retries, defaults to 10  


#### (optional) delay  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Incremental delay increase in milliseconds  


#### (optional) userAgent  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;User-Agent string to set  


## See also
- [PnPHttpProvider](OfficeDevPnP.Core.Utilities.PnPHttpProvider.md)
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)
