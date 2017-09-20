# FieldAndContentTypeExtensions.SetDefaultContentTypeToList Method  
 Set's default content type list.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetDefaultContentTypeToList(this List list, String contentTypeId)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;List to update  

  

#### contentTypeId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Complete ID for the content type  

  

### Return Value
Type: void  

## Remarks
Notice. Currently removes other content types from the list. Known issue
  
## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
