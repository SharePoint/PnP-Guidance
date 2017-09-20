# TenantExtensions.SetSiteLockState Method  
 Sets a site to Unlock access or NoAccess. This operation may occur immediately, but the site lock may take a short while before it goes into effect.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetSiteLockState(this Tenant tenant, String siteFullUrl, SiteLockState lockState, Boolean wait = False, Func<TenantOperationMessage, Boolean> timeoutFunction)
```
### Parameters
#### tenant  
&emsp;&emsp;Type: Microsoft.Online.SharePoint.TenantAdministration.Tenant  
&emsp;&emsp;A tenant object pointing to the context of a Tenant Administration site (i.e. https://[tenant]-admin.sharepoint.com)  

  

#### siteFullUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The target site to change the lock state.  

  

#### lockState  
&emsp;&emsp;Type: [OfficeDevPnP.Core.SiteLockState](OfficeDevPnP.Core.SiteLockState.md)  
&emsp;&emsp;The target state the site should be changed to.  

  

#### (optional) wait  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;If true, processing will halt until the site collection lock state has been implemented  

  

#### (optional) timeoutFunction  
&emsp;&emsp;Type: System.Func&lt;OfficeDevPnP.Core.TenantOperationMessage, System.Boolean&gt;  
&emsp;&emsp;An optional function that will be called while waiting for the site to be created. If set will override the wait variable. Return true to cancel the wait loop.  

  

### Return Value
Type: void  

## See also
- [TenantExtensions](Microsoft.SharePoint.Client.TenantExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
