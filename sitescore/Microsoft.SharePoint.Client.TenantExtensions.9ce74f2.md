# TenantExtensions.GetSiteCollections Method  
 Returns all site collections in the current Tenant based on a startIndex. IncludeDetail adds additional properties to the SPSite object.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static IList<SiteEntity> GetSiteCollections(this Tenant tenant, Int32 startIndex = 0, Int32 endIndex = 500000, Boolean includeDetail = True, Boolean includeOD4BSites = False)
```
### Parameters
#### tenant  
&emsp;&emsp;Type: Microsoft.Online.SharePoint.TenantAdministration.Tenant  
&emsp;&emsp;Tenant object to operate against  

  

#### (optional) startIndex  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Not relevant anymore  

  

#### (optional) endIndex  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Not relevant anymore  

  

#### (optional) includeDetail  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Option to return a limited set of data  

  

#### (optional) includeOD4BSites  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Also return the OD4B sites  

  

### Return Value
Type: IList<SiteEntity>  
An IList of SiteEntity objects  


## See also
- [TenantExtensions](Microsoft.SharePoint.Client.TenantExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
