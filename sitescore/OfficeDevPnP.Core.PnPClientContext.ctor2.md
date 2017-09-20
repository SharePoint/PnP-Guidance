# PnPClientContext.PnPClientContext members 
 Creates a ClientContext allowing you to override the default retry and delay values of ExecuteQueryRetry   

**Namespace:** [OfficeDevPnP.Core](OfficeDevPnP.Core.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public PnPClientContext(Uri uri, int retryCount, int delay)
```
### Parameters
#### uri  
&emsp;&emsp;Type: System.Uri  
&emsp;&emsp;A SharePoint site/web full url  


#### (optional) retryCount  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Maximum amount of retries before giving up  


#### (optional) delay  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Initial delay in milliseconds  


## See also
- [PnPClientContext](OfficeDevPnP.Core.PnPClientContext.md)
- [OfficeDevPnP.Core](OfficeDevPnP.Core.md)
