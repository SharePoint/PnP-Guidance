# WebAPIHelper.HasCacheEntry Method  
 Checks if this request has a servicesToken cookie. To be used from inside the WebAPI.   

**Namespace:** [OfficeDevPnP.Core.WebAPI](OfficeDevPnP.Core.WebAPI.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool HasCacheEntry(HttpControllerContext httpControllerContext)
```
### Parameters
#### httpControllerContext  
&emsp;&emsp;Type: System.Web.Http.Controllers.HttpControllerContext  
&emsp;&emsp;Information about the HTTP request that reached the WebAPI controller  

  

### Return Value
Type: bool  
True if cookie is available and not empty, false otherwise  


## See also
- [WebAPIHelper](OfficeDevPnP.Core.WebAPI.WebAPIHelper.md) 
- [OfficeDevPnP.Core.WebAPI](OfficeDevPnP.Core.WebAPI.md) 
