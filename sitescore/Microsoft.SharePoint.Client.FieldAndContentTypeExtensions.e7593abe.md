# FieldAndContentTypeExtensions.SetLocalizationForContentType Method  
 Set localized labels for content type   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetLocalizationForContentType(this ContentType contentType, String cultureName, String nameResource, String descriptionResource)
```
### Parameters
#### contentType  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ContentType  
&emsp;&emsp;Name of the content type  

  

#### cultureName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Culture for the localization (en-es, nl-be, fi-fi,...)  

  

#### nameResource  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Localized value for the Name property  

  

#### descriptionResource  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Localized value for the Description property  

  

### Return Value
Type: void  

## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
