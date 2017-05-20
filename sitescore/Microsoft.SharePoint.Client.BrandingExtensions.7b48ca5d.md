# BrandingExtensions.SetMasterPageByUrl Method  
 Set master page by using given URL as parameter. Suitable for example in cases where you want sub sites to reference root site master page gallery. This is typical with publishing sites.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetMasterPageByUrl(this Web web, String masterPageServerRelativeUrl, Boolean resetSubsitesToInherit = False, Boolean updateRootOnly = False)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Context web  

  

#### masterPageServerRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;URL to the master page.  

  

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
