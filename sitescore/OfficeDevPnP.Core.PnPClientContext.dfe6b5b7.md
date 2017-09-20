# PnPClientContext.ConvertFrom Method  
 Converts ClientContext into PnPClientContext   

**Namespace:** [OfficeDevPnP.Core](OfficeDevPnP.Core.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static PnPClientContext ConvertFrom(ClientContext clientContext, Int32 retryCount = 10, Int32 delay = 500)
```
### Parameters
#### clientContext  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ClientContext  
&emsp;&emsp;A SharePoint ClientContext for resource operations  

  

#### (optional) retryCount  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Maximum amount of retries before giving up  

  

#### (optional) delay  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Initial delay in milliseconds  

  

### Return Value
Type: [PnPClientContext](OfficeDevPnP.Core.PnPClientContext.md)  
  


## See also
- [PnPClientContext](OfficeDevPnP.Core.PnPClientContext.md) 
- [OfficeDevPnP.Core](OfficeDevPnP.Core.md) 
