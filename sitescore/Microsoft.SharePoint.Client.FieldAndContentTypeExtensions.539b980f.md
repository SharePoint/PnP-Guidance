# FieldAndContentTypeExtensions.AddFieldToContentTypeByName Method  
 Associates field to content type   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddFieldToContentTypeByName(this Web web, String contentTypeName, Guid fieldID, Boolean required = False, Boolean hidden = False)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### contentTypeName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the content type  

  

#### fieldID  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;Guid representation of the field ID  

  

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
