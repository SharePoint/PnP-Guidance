# PnPClientContext Class
 Class that deals with PnPClientContext methods   

**Namespace:** [OfficeDevPnP.Core](OfficeDevPnP.Core.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;Microsoft.SharePoint.Client.ClientContext  
## Syntax
```C#
public class PnPClientContext: ClientContext
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [PnPClientContext(String, Int32, Int32)](OfficeDevPnP.Core.PnPClientContext.ctor1.md) | Creates a ClientContext allowing you to override the default retry and delay values of ExecuteQueryRetry 
| [PnPClientContext(Uri, Int32, Int32)](OfficeDevPnP.Core.PnPClientContext.ctor2.md) | Creates a ClientContext allowing you to override the default retry and delay values of ExecuteQueryRetry 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [Delay](OfficeDevPnP.Core.PnPClientContext.Delay.md) | 
| [RetryCount](OfficeDevPnP.Core.PnPClientContext.RetryCount.md) | 
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Clone(String)](OfficeDevPnP.Core.PnPClientContext.4c031e75.md) | Clones a PnPClientContext object while "taking over" the security context of the existing PnPClientContext instance
| [Clone(Uri)](OfficeDevPnP.Core.PnPClientContext.d4f8ecbb.md) | Clones a PnPClientContext object while "taking over" the security context of the existing PnPClientContext instance
| [ConvertFrom(ClientContext, Int32, Int32)](OfficeDevPnP.Core.PnPClientContext.dfe6b5b7.md) | Converts ClientContext into PnPClientContext
## See also
- [OfficeDevPnP.Core](OfficeDevPnP.Core.md)
