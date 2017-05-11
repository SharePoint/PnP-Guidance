# TenantExtensions.SetSiteProperties Method  
 Sets tenant site Properties   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetSiteProperties(Tenant tenant, String siteFullUrl, String title, Nullable<Boolean> allowSelfServiceUpgrade, Nullable<SharingCapabilities> sharingCapability, Nullable<Int64> storageMaximumLevel, Nullable<Int64> storageWarningLevel, Nullable<Double> userCodeMaximumLevel, Nullable<Double> userCodeWarningLevel, Nullable<Boolean> noScriptSite, Boolean wait, Func<TenantOperationMessage, Boolean> timeoutFunction)
```
### Parameters
#### tenant  
&emsp;&emsp;Type: Microsoft.Online.SharePoint.TenantAdministration.Tenant  
&emsp;&emsp;A tenant object pointing to the context of a Tenant Administration site  

  

#### siteFullUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp; Sets tenant site Properties   

  

#### (optional) title  
&emsp;&emsp;Type: System.String  
&emsp;&emsp; Sets tenant site Properties   

  

#### (optional) allowSelfServiceUpgrade  
&emsp;&emsp;Type: System.Nullable<System.Boolean>  
&emsp;&emsp; Sets tenant site Properties   

  

#### (optional) sharingCapability  
&emsp;&emsp;Type: System.Nullable<Microsoft.Online.SharePoint.TenantManagement.SharingCapabilities>  
&emsp;&emsp; Sets tenant site Properties   

  

#### (optional) storageMaximumLevel  
&emsp;&emsp;Type: System.Nullable<System.Int64>  
&emsp;&emsp; Sets tenant site Properties   

  

#### (optional) storageWarningLevel  
&emsp;&emsp;Type: System.Nullable<System.Int64>  
&emsp;&emsp; Sets tenant site Properties   

  

#### (optional) userCodeMaximumLevel  
&emsp;&emsp;Type: System.Nullable<System.Double>  
&emsp;&emsp; Sets tenant site Properties   

  

#### (optional) userCodeWarningLevel  
&emsp;&emsp;Type: System.Nullable<System.Double>  
&emsp;&emsp; Sets tenant site Properties   

  

#### (optional) noScriptSite  
&emsp;&emsp;Type: System.Nullable<System.Boolean>  
&emsp;&emsp; Sets tenant site Properties   

  

#### (optional) wait  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp; Sets tenant site Properties   

  

#### (optional) timeoutFunction  
&emsp;&emsp;Type: System.Func<OfficeDevPnP.Core.TenantOperationMessage, System.Boolean>  
&emsp;&emsp; Sets tenant site Properties   

  

### Return Value
Type: void  

## Remarks
  
## See also
- [TenantExtensions](Microsoft.SharePoint.Client.TenantExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
