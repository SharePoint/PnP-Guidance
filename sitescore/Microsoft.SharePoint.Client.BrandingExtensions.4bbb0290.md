# BrandingExtensions.SetThemeByUrl Method  
 Recursively applies the specified palette, font, and background image.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetThemeByUrl(this Web web, String paletteServerRelativeUrl, String fontServerRelativeUrl, String backgroundServerRelativeUrl, Boolean resetSubsitesToInherit = False, Boolean updateRootOnly = False)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to apply to  

  

#### paletteServerRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;URL of palette file to apply  

  

#### fontServerRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;URL of font file to apply  

  

#### backgroundServerRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;URL of background image to apply  

  

#### (optional) resetSubsitesToInherit  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;false (default) to apply to currently inheriting subsites only; true to force all subsites to inherit  

  

#### (optional) updateRootOnly  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;false (default) to apply to subsites; true to only apply to specified site  

  

### Return Value
Type: void  

## See also
- [BrandingExtensions](Microsoft.SharePoint.Client.BrandingExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
