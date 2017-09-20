# BrandingExtensions.GetComposedLook Method  
 Returns the named composed look from the web gallery   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static ThemeEntity GetComposedLook(this Web web, String composedLookName)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to check  

  

#### composedLookName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the composed look to retrieve  

  

### Return Value
Type: [ThemeEntity](OfficeDevPnP.Core.Entities.ThemeEntity.md)  
Entity with the attributes of the composed look, or null if the composed look does not exists or cannot be determined  


## See also
- [BrandingExtensions](Microsoft.SharePoint.Client.BrandingExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
