# SecurityExtensions.GetSharingCapabilitiesTenant Method  
 Get the external sharing settings for the provided site. Only works in Office 365 Multi-Tenant   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static string GetSharingCapabilitiesTenant(this Web web, Uri siteUrl)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Tenant administration web  

  

#### siteUrl  
&emsp;&emsp;Type: System.Uri  
&emsp;&emsp;Site to get the sharing capabilities from  

  

### Return Value
Type: string  
Sharing capabilities of the site collection  


## See also
- [SecurityExtensions](Microsoft.SharePoint.Client.SecurityExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
