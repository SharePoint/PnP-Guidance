# BrandingExtensions.CreateComposedLookByUrl Method  
 Creates (or updates) a composed look in the web site; usually this is done in the root site of the collection.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void CreateComposedLookByUrl(this Web web, String lookName, String paletteServerRelativeUrl, String fontServerRelativeUrl, String backgroundServerRelativeUrl, String masterServerRelativeUrl, Int32 displayOrder = 1, Boolean replaceContent = True)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to create the composed look in  

  

#### lookName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the theme  

  

#### paletteServerRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;URL of the palette file, usually in the theme catalog of the site collection  

  

#### fontServerRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;URL of the font file, usually in the theme catalog of the site collection  

  

#### backgroundServerRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;URL of the background image file, usually in /_layouts/15/images  

  

#### masterServerRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;URL of the master page, usually in the masterpage catalog of the web site  

  

#### (optional) displayOrder  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Display order of the composed look  

  

#### (optional) replaceContent  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Replace composed look if it already exists (default true)  

  

### Return Value
Type: void  

## See also
- [BrandingExtensions](Microsoft.SharePoint.Client.BrandingExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
