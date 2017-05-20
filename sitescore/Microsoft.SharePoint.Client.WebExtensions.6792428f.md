# WebExtensions.CreateWeb Method  
 Adds a new child Web (site) to a parent Web.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Web CreateWeb(this Web parentWeb, SiteEntity subsite, Boolean inheritPermissions = True, Boolean inheritNavigation = True)
```
### Parameters
#### parentWeb  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The parent Web (site) to create under  

  

#### subsite  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Entities.SiteEntity](OfficeDevPnP.Core.Entities.SiteEntity.md)  
&emsp;&emsp;Details of the Web (site) to add. Only Title, Url (as the leaf URL), Description, Template and Language are used.  

  

#### (optional) inheritPermissions  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Specifies whether the new site will inherit permissions from its parent site.  

  

#### (optional) inheritNavigation  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Specifies whether the site inherits navigation.  

  

### Return Value
Type: Web  
  


## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
