# BrandingExtensions.CreateComposedLookByName Method  
 Creates (or updates) a composed look in the web site; usually this is done in the root site of the collection.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void CreateComposedLookByName(this Web web, String lookName, String paletteFileName, String fontFileName, String backgroundFileName, String masterFileName, Int32 displayOrder = 1, Boolean replaceContent = True)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to create the composed look in  

  

#### lookName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the theme  

  

#### paletteFileName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;File name of the palette file in the theme catalog of the site collection; path component ignored.  

  

#### fontFileName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;File name of the font file in the theme catalog of the site collection; path component ignored.  

  

#### backgroundFileName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;File name of the background image file in the theme catalog of the site collection; path component ignored.  

  

#### masterFileName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;File name of the master page in the mastepage catalog of the web site; path component ignored.  

  

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
