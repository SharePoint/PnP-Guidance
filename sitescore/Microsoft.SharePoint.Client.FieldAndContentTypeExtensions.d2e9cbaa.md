# FieldAndContentTypeExtensions.AddContentTypeToListById Method  
 Add content type to list   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool AddContentTypeToListById(this List list, String contentTypeID, Boolean defaultContent = False, Boolean searchContentTypeInSiteHierarchy = False)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;List to add content type to  

  

#### contentTypeID  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Complete ID for the content type  

  

#### (optional) defaultContent  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;If set true, content type is updated to be default content type for the list  

  

#### (optional) searchContentTypeInSiteHierarchy  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;search for content type in site hierarchy  

  

### Return Value
Type: bool  

## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
