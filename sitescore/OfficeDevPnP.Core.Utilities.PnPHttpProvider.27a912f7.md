# PnPHttpProvider.SendAsync Method  
 Perform async http request   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public override Task<HttpResponseMessage> SendAsync(HttpRequestMessage request, CancellationToken cancellationToken)
```
### Parameters
#### request  
&emsp;&emsp;Type: System.Net.Http.HttpRequestMessage  
&emsp;&emsp;Http request to execute  

  

#### cancellationToken  
&emsp;&emsp;Type: System.Threading.CancellationToken  
&emsp;&emsp;cancellation token  

  

### Return Value
Type: Task<HttpResponseMessage>  
Response object from http request  


## See also
- [PnPHttpProvider](OfficeDevPnP.Core.Utilities.PnPHttpProvider.md) 
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md) 
