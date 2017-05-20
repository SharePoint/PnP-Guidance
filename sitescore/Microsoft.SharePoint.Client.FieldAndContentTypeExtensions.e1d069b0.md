# FieldAndContentTypeExtensions.BestMatch Method  
 Searches for the content type with the closest match to the value of the specified content type ID. If the search finds two matches, the shorter ID is returned.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static ContentTypeId BestMatch(this ContentTypeCollection contentTypes, String contentTypeId)
```
### Parameters
#### contentTypes  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ContentTypeCollection  
&emsp;&emsp;Content type collection to search  

  

#### contentTypeId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Complete ID for the content type to search  

  

### Return Value
Type: ContentTypeId  
Content type Id object or null if was not found  


## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
