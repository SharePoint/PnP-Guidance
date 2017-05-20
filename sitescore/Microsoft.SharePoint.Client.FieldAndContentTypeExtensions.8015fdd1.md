# FieldAndContentTypeExtensions.AddContentTypeToList Method  
 Adds content type to list   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddContentTypeToList(this Web web, String listTitle, ContentType contentType, Boolean defaultContent = False)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### listTitle  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Title of the list  

  

#### contentType  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ContentType  
&emsp;&emsp;Content type to be added to the list  

  

#### (optional) defaultContent  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;If set true, content type is updated to be default content type for the list  

  

### Return Value
Type: void  

## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
