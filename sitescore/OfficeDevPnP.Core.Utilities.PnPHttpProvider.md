# PnPHttpProvider Class
 PnP http client which implements setting of User-Agent + retry mechanismn on throttling   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;System.Net.Http.HttpClient  
## Syntax
```C#
public class PnPHttpProvider: HttpClient
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [PnPHttpProvider(Int32, Int32, String)](OfficeDevPnP.Core.Utilities.PnPHttpProvider.ctor1.md) | Constructor without HttpMessageHandler 
| [PnPHttpProvider(HttpMessageHandler, Int32, Int32, String)](OfficeDevPnP.Core.Utilities.PnPHttpProvider.ctor2.md) | Constructor with HttpMessageHandler 
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [SendAsync(HttpRequestMessage, CancellationToken)](OfficeDevPnP.Core.Utilities.PnPHttpProvider.27a912f7.md) | Perform async http request
## See also
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)
