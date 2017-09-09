# TenantExtensions.DeployApplicationPackageToAppCatalog Method  
 Adds a package to the tenants app catalog and by default deploys it if the package is a client side package (sppkg)   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  

>**This method is obsolete**
>:Please use the DeployApplicationPackageToAppCatalog extension method on the Web class. This method will be removed in the October 2017 release.

## Syntax
```C#
public static ListItem DeployApplicationPackageToAppCatalog(this Tenant tenant, String spPkgName, String spPkgPath, Boolean autoDeploy = True, Boolean skipFeatureDeployment = True, Boolean overwrite = True)
```
### Parameters
#### tenant  
&emsp;&emsp;Type: Microsoft.Online.SharePoint.TenantAdministration.Tenant  
&emsp;&emsp;Tenant to operate against  

  

#### spPkgName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the package to upload (e.g. demo.sppkg)   

  

#### spPkgPath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Path on the filesystem where this package is stored  

  

#### (optional) autoDeploy  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Automatically deploy the package, only applies to client side packages (sppkg)  

  

#### (optional) skipFeatureDeployment  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Skip the feature deployment step, allows for a one-time central deployment of your solution  

  

#### (optional) overwrite  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Overwrite the package if it was already listed in the app catalog  

  

### Return Value
Type: ListItem  
The ListItem of the added package row  


## See also
- [TenantExtensions](Microsoft.SharePoint.Client.TenantExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
