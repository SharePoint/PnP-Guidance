# FieldAndContentTypeExtensions.ReorderContentTypes Method  
 Reorders content types on the list. The first one in the list is the default item. Any items left out from the list will still be on the content type, but will not be visible on the new button.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void ReorderContentTypes(this List list, IEnumerable<String> contentTypeNamesOrIds)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;Target list containing the content types  

  

#### contentTypeNamesOrIds  
&emsp;&emsp;Type: System.Collections.Generic.IEnumerable&lt;System.String&gt;  
&emsp;&emsp;Content type names or ids to sort.  

  

### Return Value
Type: void  

## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
