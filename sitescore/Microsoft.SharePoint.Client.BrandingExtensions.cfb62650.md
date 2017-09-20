# BrandingExtensions.SetComposedLookByUrl Method  
 Retrieves the named composed look, overrides with specified palette, font, background and master page, and then recursively sets the specified values.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetComposedLookByUrl(this Web web, String lookName, String paletteServerRelativeUrl, String fontServerRelativeUrl, String backgroundServerRelativeUrl, String masterServerRelativeUrl, Boolean resetSubsitesToInherit = False, Boolean updateRootOnly = True)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to apply composed look to  

  

#### lookName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the composed look to apply; null will apply the override values only  

  

#### (optional) paletteServerRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Override palette file URL to use  

  

#### (optional) fontServerRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Override font file URL to use  

  

#### (optional) backgroundServerRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Override background image file URL to use  

  

#### (optional) masterServerRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Override master page file URL to use  

  

#### (optional) resetSubsitesToInherit  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;false (default) to apply to currently inheriting subsites only; true to force all subsites to inherit  

  

#### (optional) updateRootOnly  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;false to apply to subsites; true (default) to only apply to specified site  

  

### Return Value
Type: void  

## See also
- [BrandingExtensions](Microsoft.SharePoint.Client.BrandingExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
