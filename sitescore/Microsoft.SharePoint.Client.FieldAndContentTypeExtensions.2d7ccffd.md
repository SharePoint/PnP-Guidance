# FieldAndContentTypeExtensions.SetLocalizationForField Method  
 Set localized labels for field   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetLocalizationForField(this Field field, String cultureName, String titleResource, String descriptionResource)
```
### Parameters
#### field  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Field  
&emsp;&emsp;Field to update  

  

#### cultureName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Culture for the localization (en-es, nl-be, fi-fi,...)  

  

#### titleResource  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Localized value for the Title property  

  

#### descriptionResource  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Localized value for the Description property  

  

### Return Value
Type: void  

## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
