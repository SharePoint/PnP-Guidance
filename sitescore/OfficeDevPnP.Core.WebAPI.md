# OfficeDevPnP.Core.WebAPI
## Classes
|**Class**|**Description**|
|:-----|:-----|
|[WebAPIContexCacheItem](OfficeDevPnP.Core.WebAPI.WebAPIContexCacheItem.md)|This class holds the information that's being cached as part of the WebAPI service implementation|
|[WebAPIContext](OfficeDevPnP.Core.WebAPI.WebAPIContext.md)|This class holds the information that's passed from the SharePoint app to the "Register" WebAPI service call|
|[WebAPIContextCache](OfficeDevPnP.Core.WebAPI.WebAPIContextCache.md)| Simple cache implementation based on the singleton pattern. Caches the SharePoint access token, refresh token and the information passed during service "registration". All of this information is wrapped in a T:OfficeDevPnP.Core.WebAPI.WebAPIContexCacheItem object. |
|[WebAPIContextFilterAttribute](OfficeDevPnP.Core.WebAPI.WebAPIContextFilterAttribute.md)|Class deals with WebAPI context filter attribute and excutes action based on HttpActionContext|
|[WebAPIHelper](OfficeDevPnP.Core.WebAPI.WebAPIHelper.md)|This class provides helper methods that can be used to protect WebAPI services and to provide a way to reinstantiate a contextobject in the service call.|
