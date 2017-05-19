# WebAPIHelper.GetClientContext Method  
 Creates a ClientContext token for the incoming WebAPI request. This is done by - looking up the servicesToken - extracting the cacheKey - get the AccessToken from cache. If the AccessToken is expired a new one is requested using the refresh token - creation of a ClientContext object based on the AccessToken   

**Namespace:** [OfficeDevPnP.Core.WebAPI](OfficeDevPnP.Core.WebAPI.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static ClientContext GetClientContext(HttpControllerContext httpControllerContext)
```
### Parameters
#### httpControllerContext  
&emsp;&emsp;Type: System.Web.Http.Controllers.HttpControllerContext  
&emsp;&emsp;Information about the HTTP request that reached the WebAPI controller  

  

### Return Value
Type: ClientContext  
A valid ClientContext object  


## See also
- [WebAPIHelper](OfficeDevPnP.Core.WebAPI.WebAPIHelper.md) 
- [OfficeDevPnP.Core.WebAPI](OfficeDevPnP.Core.WebAPI.md) 
