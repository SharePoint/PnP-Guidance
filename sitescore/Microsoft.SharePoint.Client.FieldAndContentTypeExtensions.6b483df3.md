# FieldAndContentTypeExtensions.FieldExistsByNameInContentType Method  
 Field exists in content type   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool FieldExistsByNameInContentType(this Web web, String contentTypeName, String fieldName)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site. Site columns should be created to root site.  

  

#### contentTypeName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the content type  

  

#### fieldName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the field  

  

### Return Value
Type: bool  
True if exists, false otherwise  


## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
