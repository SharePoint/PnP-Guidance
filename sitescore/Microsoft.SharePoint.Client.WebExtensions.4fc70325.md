# WebExtensions.SetLocalizationLabels Method  
 Can be used to set translations for different cultures.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetLocalizationLabels(this Web web, String cultureName, String titleResource, String descriptionResource)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### cultureName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Culture name like en-us or fi-fi  

  

#### titleResource  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Localized Title string  

  

#### descriptionResource  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Localized Description string  

  

### Return Value
Type: void  

## Examples
```C#
web.SetLocalizationForSiteLabels("fi-fi", "Name of the site in Finnish", "Description in Finnish");
            
```

## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [http://blogs.msdn.com/b/vesku/archive/2014/03/20/office365-multilingual-content-types-site-columns-and-site-other-elements.aspx](http://blogs.msdn.com/b/vesku/archive/2014/03/20/office365-multilingual-content-types-site-columns-and-site-other-elements.aspx)
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
