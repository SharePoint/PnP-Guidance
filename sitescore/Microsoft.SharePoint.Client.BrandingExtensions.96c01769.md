# BrandingExtensions.GetPageLayoutListItemByName Method  
 Gets a page layout from the master page catalog. Can be called with paramter as "pagelayout.aspx" or as full path like "_catalog/masterpage/pagelayout.aspx"   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static ListItem GetPageLayoutListItemByName(this Web web, String pageLayoutName)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;root web  

  

#### pageLayoutName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;name of the page layout to retrieve  

  

### Return Value
Type: ListItem  
ListItem holding the page layout, null if not found  


## See also
- [BrandingExtensions](Microsoft.SharePoint.Client.BrandingExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
