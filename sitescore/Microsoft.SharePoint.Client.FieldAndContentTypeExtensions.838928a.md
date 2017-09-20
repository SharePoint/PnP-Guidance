# FieldAndContentTypeExtensions.CreateContentType Method  
 Create new content type to web   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static ContentType CreateContentType(this Web web, String name, String description, String id, String group, ContentType parentContentType)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### name  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the content type  

  

#### description  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Description for the content type  

  

#### id  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Complete ID for the content type  

  

#### group  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Group for the content type  

  

#### (optional) parentContentType  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ContentType  
&emsp;&emsp;Parent Content Type  

  

### Return Value
Type: ContentType  
The created content type  


## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
