# TenantExtensions.CreateSiteCollection Method  
 Adds a SiteEntity by launching site collection creation and waits for the creation to finish   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Guid CreateSiteCollection(this Tenant tenant, SiteEntity properties, Boolean removeFromRecycleBin = False, Boolean wait = True, Func<TenantOperationMessage, Boolean> timeoutFunction)
```
### Parameters
#### tenant  
&emsp;&emsp;Type: Microsoft.Online.SharePoint.TenantAdministration.Tenant  
&emsp;&emsp;A tenant object pointing to the context of a Tenant Administration site  

  

#### properties  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Entities.SiteEntity](OfficeDevPnP.Core.Entities.SiteEntity.md)  
&emsp;&emsp;Describes the site collection to be created  

  

#### (optional) removeFromRecycleBin  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;It true and site is present in recycle bin, it will be removed first from the recycle bin  

  

#### (optional) wait  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;If true, processing will halt until the site collection has been created  

  

#### (optional) timeoutFunction  
&emsp;&emsp;Type: System.Func&lt;OfficeDevPnP.Core.TenantOperationMessage, System.Boolean&gt;  
&emsp;&emsp;An optional function that will be called while waiting for the site to be created. If set will override the wait variable. Return true to cancel the wait loop.  

  

### Return Value
Type: Guid  
Guid of the created site collection and Guid.Empty is the wait parameter is specified as false. Returns Guid.Empty if the wait is cancelled.  


## See also
- [TenantExtensions](Microsoft.SharePoint.Client.TenantExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
