# TenantExtensions.DeleteSiteCollectionFromRecycleBin Method  
 Deletes a site collection from the site collection recycle bin   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool DeleteSiteCollectionFromRecycleBin(this Tenant tenant, String siteFullUrl, Boolean wait = True, Func<TenantOperationMessage, Boolean> timeoutFunction)
```
### Parameters
#### tenant  
&emsp;&emsp;Type: Microsoft.Online.SharePoint.TenantAdministration.Tenant  
&emsp;&emsp;A tenant object pointing to the context of a Tenant Administration site  

  

#### siteFullUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;URL of the site collection to delete  

  

#### (optional) wait  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;If true, processing will halt until the site collection has been deleted from the recycle bin  

  

#### (optional) timeoutFunction  
&emsp;&emsp;Type: System.Func&lt;OfficeDevPnP.Core.TenantOperationMessage, System.Boolean&gt;  
&emsp;&emsp;An optional function that will be called while waiting for the site to be created. If set will override the wait variable. Return true to cancel the wait loop.  

  

### Return Value
Type: bool  

## See also
- [TenantExtensions](Microsoft.SharePoint.Client.TenantExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
