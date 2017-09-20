# TenantExtensions.DeleteSiteCollection Method  
 Deletes a site collection   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool DeleteSiteCollection(this Tenant tenant, String siteFullUrl, Boolean useRecycleBin, Func<TenantOperationMessage, Boolean> timeoutFunction)
```
### Parameters
#### tenant  
&emsp;&emsp;Type: Microsoft.Online.SharePoint.TenantAdministration.Tenant  
&emsp;&emsp;A tenant object pointing to the context of a Tenant Administration site  

  

#### siteFullUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Url of the site collection to delete  

  

#### useRecycleBin  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Leave the deleted site collection in the site collection recycle bin  

  

#### (optional) timeoutFunction  
&emsp;&emsp;Type: System.Func&lt;OfficeDevPnP.Core.TenantOperationMessage, System.Boolean&gt;  
&emsp;&emsp;An optional function that will be called while waiting for the site to be created. Return true to cancel the wait loop.  

  

### Return Value
Type: bool  
True if deleted  


## See also
- [TenantExtensions](Microsoft.SharePoint.Client.TenantExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
