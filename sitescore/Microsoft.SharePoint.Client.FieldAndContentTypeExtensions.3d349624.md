# FieldAndContentTypeExtensions.AddFieldToContentType Method  
 Associates field to content type   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddFieldToContentType(this Web web, ContentType contentType, Field field, Boolean required = False, Boolean hidden = False)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### contentType  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ContentType  
&emsp;&emsp;Content type to associate field to  

  

#### field  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Field  
&emsp;&emsp;Field to associate to the content type  

  

#### (optional) required  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Optionally make this a required field  

  

#### (optional) hidden  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Optionally make this a hidden field  

  

### Return Value
Type: void  

## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
