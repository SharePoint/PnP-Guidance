# FieldAndContentTypeExtensions.SetLocalizationForField Method  
 Set localized labels for field   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetLocalizationForField(this List list, String siteColumnName, String cultureName, String titleResource, String descriptionResource)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;List to update  

  

#### siteColumnName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the site column  

  

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
