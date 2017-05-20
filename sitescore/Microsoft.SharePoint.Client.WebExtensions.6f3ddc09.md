# WebExtensions.SetPageOutputCache Method  
 Sets output cache on publishing web. The settings can be maintained from UI by visiting url /_layouts/15/sitecachesettings.aspx   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetPageOutputCache(this Web web, Boolean enableOutputCache, Int32 anonymousCacheProfileId, Int32 authenticatedCacheProfileId, Boolean debugCacheInformation)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;SharePoint web  

  

#### enableOutputCache  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Specify true to enable output cache. False otherwise.  

  

#### anonymousCacheProfileId  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Applies for anonymous users access for a site in Site Collection. Id of the profile specified in "Cache Profiles" list.  

  

#### authenticatedCacheProfileId  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Applies for authenticated users access for a site in the Site Collection. Id of the profile specified in "Cache Profiles" list.  

  

#### debugCacheInformation  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Specify true to enable the display of additional cache information on pages in this site collection. False otherwise.  

  

### Return Value
Type: void  

## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
