# FieldAndContentTypeExtensions.AddFieldToContentTypeById Method  
 Associates field to content type   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddFieldToContentTypeById(this Web web, String contentTypeID, String fieldId, Boolean required = False, Boolean hidden = False)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### contentTypeID  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;String representation of the id of the content type to add the field to  

  

#### fieldId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;String representation of the field ID (=guid)  

  

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
