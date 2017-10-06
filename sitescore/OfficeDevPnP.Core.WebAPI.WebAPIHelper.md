# WebAPIHelper Class
 This class provides helper methods that can be used to protect WebAPI services and to provide a way to reinstantiate a contextobject in the service call.   

**Namespace:** [OfficeDevPnP.Core.WebAPI](OfficeDevPnP.Core.WebAPI.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class WebAPIHelper
```
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [AddToCache(WebAPIContext)](OfficeDevPnP.Core.WebAPI.WebAPIHelper.10fa47cc.md) | Uses the information regarding the requesting app to obtain an access token and caches that using the cachekey. This method is called from the Register WebAPI service api.
| [GetClientContext(HttpControllerContext)](OfficeDevPnP.Core.WebAPI.WebAPIHelper.291cca75.md) | Creates a ClientContext token for the incoming WebAPI request. This is done by - looking up the servicesToken - extracting the cacheKey - get the AccessToken from cache. If the AccessToken is expired a new one is requested using the refresh token - creation of a ClientContext object based on the AccessToken
| [HasCacheEntry(HttpControllerContext)](OfficeDevPnP.Core.WebAPI.WebAPIHelper.c4059705.md) | Checks if this request has a servicesToken cookie. To be used from inside the WebAPI.
| [RegisterWebAPIService(HttpContextBase, String, Uri)](OfficeDevPnP.Core.WebAPI.WebAPIHelper.b0ad5e8d.md) | This method needs to be called from a code behind of the SharePoint app startup page (default.aspx). It registers the calling SharePoint app by calling a specific "Register" api in your WebAPI service. Note: Given that method is async you'll need to add the Async="true" page directive to the page that uses this method.
## Extension Methods
|**Name**|**Description**|
|:-----|:-----|
| [RegisterWebAPIService(Page, String, Uri)](OfficeDevPnP.Core.WebAPI.WebAPIHelper.ca213228.md) | This method needs to be called from a code behind of the SharePoint app startup page (default.aspx). It registers the calling SharePoint app by calling a specific "Register" api in your WebAPI service. Note: Given that method is async you'll need to add the Async="true" page directive to the page that uses this method.
## See also
- [OfficeDevPnP.Core.WebAPI](OfficeDevPnP.Core.WebAPI.md)
