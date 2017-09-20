# FieldAndContentTypeExtensions.SetJsLinkCustomizations Method  
 Adds jsLink to a field.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetJsLinkCustomizations(this Field field, String jsLink)
```
### Parameters
#### field  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Field  
&emsp;&emsp;The field to add jsLink to  

  

#### jsLink  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;JSLink to set to the form. Set to empty string to remove the set JSLink customization. Specify multiple values separated by pipe symbol. For e.g.: ~sitecollection/_catalogs/masterpage/jquery-2.1.0.min.js|~sitecollection/_catalogs/masterpage/custom.js   

  

### Return Value
Type: void  

## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
