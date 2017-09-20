# FieldAndContentTypeExtensions.BestMatchContentTypeId Method  
 Searches the list content types and returns the content type identifier (ID) that is the nearest match to the specified content type ID.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static ContentTypeId BestMatchContentTypeId(this List list, String baseContentTypeId)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;The list to check for content types  

  

#### baseContentTypeId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;A string with the base content type ID to match.  

  

### Return Value
Type: ContentTypeId  
The value of the Id property for the content type with the closest match to the value of the specified content type ID.   


## Remarks
 If the search finds multiple matches, the shorter ID is returned. For example, if 0x0101 is the argument, and the collection contains both 0x010109 and 0x01010901, the method returns 0x010109. 
  
## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
