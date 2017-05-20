# FieldAndContentTypeExtensions.AddFieldById Method  
 Associates field to content type   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddFieldById(this ContentType contentType, Guid fieldId, Boolean required = False, Boolean hidden = False)
```
### Parameters
#### contentType  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ContentType  
&emsp;&emsp;Content Type to add the field to  

  

#### fieldId  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;The Id of the field  

  

#### (optional) required  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;True if the field is required  

  

#### (optional) hidden  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;True if the field is hidden  

  

### Return Value
Type: void  

## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
