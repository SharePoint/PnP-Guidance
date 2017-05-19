# WebAPIContextCache Class
Simple cache implementation based on the singleton pattern. Caches the SharePoint access token, refresh token and the information passed during service "registration". All of this information is wrapped in a  [OfficeDevPnP.Core.WebAPI.WebAPIContexCacheItem](OfficeDevPnP.Core.WebAPI.WebAPIContexCacheItem.md)  object  

**Namespace:** [OfficeDevPnP.Core.WebAPI](OfficeDevPnP.Core.WebAPI.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public class WebAPIContextCache
```
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [Instance](OfficeDevPnP.Core.WebAPI.WebAPIContextCache.Instance.md) | Singleton instance to access this class
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Get(String)](OfficeDevPnP.Core.WebAPI.WebAPIContextCache.c451aec8.md) | Gets an item from the cache
| [Put(String, WebAPIContexCacheItem)](OfficeDevPnP.Core.WebAPI.WebAPIContextCache.47ca96e2.md) | Adds an item to the cache. Updates if the item already existed
## See also
- [OfficeDevPnP.Core.WebAPI.WebAPIContexCacheItem](OfficeDevPnP.Core.WebAPI.WebAPIContexCacheItem.md)
- [OfficeDevPnP.Core.WebAPI](OfficeDevPnP.Core.WebAPI.md)
