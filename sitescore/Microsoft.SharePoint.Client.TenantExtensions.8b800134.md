# TenantExtensions.DeployApplicationPackageToAppCatalog Method  
 Adds a package to the tenants app catalog and by default deploys it if the package is a client side package (sppkg)   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static ListItem DeployApplicationPackageToAppCatalog(Tenant tenant, String appCatalogSiteUrl, String spPkgName, String spPkgPath, Boolean autoDeploy, Boolean overwrite)
```
### Parameters
#### tenant  
&emsp;&emsp;Type: Microsoft.Online.SharePoint.TenantAdministration.Tenant  
&emsp;&emsp;Tenant to operate against  

  

#### appCatalogSiteUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Full url to the tenant admin site (e.g. https://contoso.sharepoint.com/sites/apps)   

  

#### spPkgName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the package to upload (e.g. demo.sppkg)   

  

#### spPkgPath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Path on the filesystem where this package is stored  

  

#### (optional) autoDeploy  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Automatically deploy the package, only applies to client side packages (sppkg)  

  

#### (optional) overwrite  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Overwrite the package if it was already listed in the app catalog  

  

### Return Value
Type: ListItem  
The ListItem of the added package row  


## See also
- [TenantExtensions](Microsoft.SharePoint.Client.TenantExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
