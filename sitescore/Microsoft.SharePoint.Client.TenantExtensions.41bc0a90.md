# TenantExtensions.SetSiteProperties Method  
 Sets tenant site Properties   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetSiteProperties(this Tenant tenant, String siteFullUrl, String title, Nullable<Boolean> allowSelfServiceUpgrade, Nullable<SharingCapabilities> sharingCapability, Nullable<Int64> storageMaximumLevel, Nullable<Int64> storageWarningLevel, Nullable<Double> userCodeMaximumLevel, Nullable<Double> userCodeWarningLevel, Nullable<Boolean> noScriptSite, Boolean wait = True, Func<TenantOperationMessage, Boolean> timeoutFunction)
```
### Parameters
#### tenant  
&emsp;&emsp;Type: Microsoft.Online.SharePoint.TenantAdministration.Tenant  
&emsp;&emsp;A tenant object pointing to the context of a Tenant Administration site  

  

#### siteFullUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;full url of site  

  

#### (optional) title  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;site title  

  

#### (optional) allowSelfServiceUpgrade  
&emsp;&emsp;Type: System.Nullable&lt;System.Boolean&gt;  
&emsp;&emsp;Boolean value to allow serlf service upgrade  

  

#### (optional) sharingCapability  
&emsp;&emsp;Type: System.Nullable&lt;Microsoft.Online.SharePoint.TenantManagement.SharingCapabilities&gt;  
&emsp;&emsp;SharingCapabilities enumeration value (i.e. Disabled/ExternalUserSharingOnly/ExternalUserAndGuestSharing/ExistingExternalUserSharingOnly)  

  

#### (optional) storageMaximumLevel  
&emsp;&emsp;Type: System.Nullable&lt;System.Int64&gt;  
&emsp;&emsp;A limit on all disk space used by the site collection  

  

#### (optional) storageWarningLevel  
&emsp;&emsp;Type: System.Nullable&lt;System.Int64&gt;  
&emsp;&emsp;A storage warning level for when administrators of the site collection receive advance notice before available storage is expended.  

  

#### (optional) userCodeMaximumLevel  
&emsp;&emsp;Type: System.Nullable&lt;System.Double&gt;  
&emsp;&emsp;A value that represents the maximum allowed resource usage for the site/  

  

#### (optional) userCodeWarningLevel  
&emsp;&emsp;Type: System.Nullable&lt;System.Double&gt;  
&emsp;&emsp;A value that determines the level of resource usage at which a warning e-mail message is sent  

  

#### (optional) noScriptSite  
&emsp;&emsp;Type: System.Nullable&lt;System.Boolean&gt;  
&emsp;&emsp;Boolean value which allows to customize the site using scripts  

  

#### (optional) wait  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Id true this function only returns when the tenant properties are set, if false it will return immediately  

  

#### (optional) timeoutFunction  
&emsp;&emsp;Type: System.Func&lt;OfficeDevPnP.Core.TenantOperationMessage, System.Boolean&gt;  
&emsp;&emsp;An optional function that will be called while waiting for the tenant properties to be set. If set will override the wait variable. Return true to cancel the wait loop.  

  

### Return Value
Type: void  

## See also
- [TenantExtensions](Microsoft.SharePoint.Client.TenantExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
