# InformationManagementExtensions.GetSitePolicyByName Method  
 Gets the site policy with the given name   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static SitePolicyEntity GetSitePolicyByName(this Web web, String sitePolicy)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to operate on  

  

#### sitePolicy  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Site policy to fetch  

  

### Return Value
Type: [SitePolicyEntity](OfficeDevPnP.Core.Entities.SitePolicyEntity.md)  
A  [OfficeDevPnP.Core.Entities.SitePolicyEntity](OfficeDevPnP.Core.Entities.SitePolicyEntity.md)  object holding the fetched policy  


## See also
- [InformationManagementExtensions](Microsoft.SharePoint.Client.InformationManagementExtensions.md) 
- [OfficeDevPnP.Core.Entities.SitePolicyEntity](OfficeDevPnP.Core.Entities.SitePolicyEntity.md)
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
