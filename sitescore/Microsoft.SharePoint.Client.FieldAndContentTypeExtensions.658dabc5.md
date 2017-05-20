# FieldAndContentTypeExtensions.SetDefaultContentTypeToList Method  
 Set's default content type list.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetDefaultContentTypeToList(this Web web, String listTitle, ContentType contentType)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### listTitle  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Title of the list to be updated  

  

#### contentType  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ContentType  
&emsp;&emsp;Content type to make default  

  

### Return Value
Type: void  

## Remarks
Notice. Currently removes other content types from the list. Known issue
  
## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
