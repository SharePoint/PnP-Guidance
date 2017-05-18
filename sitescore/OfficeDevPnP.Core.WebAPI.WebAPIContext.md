# WebAPIContext Class
 This class holds the information that's passed from the SharePoint app to the "Register" WebAPI service call   

**Namespace:** [OfficeDevPnP.Core.WebAPI](OfficeDevPnP.Core.WebAPI.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public class WebAPIContext
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [WebAPIContext()](OfficeDevPnP.Core.WebAPI.WebAPIContext.ctor1.md) |  This class holds the information that's passed from the SharePoint app to the "Register" WebAPI service call 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [AppWebUrl](OfficeDevPnP.Core.WebAPI.WebAPIContext.AppWebUrl.md) | Url if the SharePoint app web. Needed to obtain an access token
| [CacheKey](OfficeDevPnP.Core.WebAPI.WebAPIContext.CacheKey.md) | The cacheKey that will be used. The cache key is unique for each combination of user name, user name issuer, application, and farm.
| [ClientId](OfficeDevPnP.Core.WebAPI.WebAPIContext.ClientId.md) | ClientId of the SharePoint app that's being registered. Needed to obtain an access token
| [ClientSecret](OfficeDevPnP.Core.WebAPI.WebAPIContext.ClientSecret.md) | ClientSecret of the SharePoint app that's being registered. Needed to obtain an access token
| [HostedAppHostName](OfficeDevPnP.Core.WebAPI.WebAPIContext.HostedAppHostName.md) | If the AppWebUrl is null then this value will be used. Needed to obtain an access token
| [HostWebUrl](OfficeDevPnP.Core.WebAPI.WebAPIContext.HostWebUrl.md) | Url of the SharePoint host web. Needed to obtain an access token
| [Token](OfficeDevPnP.Core.WebAPI.WebAPIContext.Token.md) | The SharePoint context token. This will be used at the WebAPI level to obtain an access token
## See also
- [OfficeDevPnP.Core.WebAPI](OfficeDevPnP.Core.WebAPI.md)
