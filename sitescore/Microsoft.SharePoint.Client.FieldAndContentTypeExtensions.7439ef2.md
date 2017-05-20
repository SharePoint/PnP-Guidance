# FieldAndContentTypeExtensions.AddFieldByName Method  
 Associates field to content type   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddFieldByName(this ContentType contentType, String fieldName, Boolean required = False, Boolean hidden = False)
```
### Parameters
#### contentType  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ContentType  
&emsp;&emsp;Content Type to add the field to  

  

#### fieldName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The title or internal name of the field  

  

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
