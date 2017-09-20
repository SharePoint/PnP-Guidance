# FieldAndContentTypeExtensions.FieldExistsById Method  
 Returns if the field is found, query based on the ID   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool FieldExistsById(this List list, String fieldId)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;List to process  

  

#### fieldId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;String representation of the field ID (=guid)  

  

### Return Value
Type: bool  
True if the fields exists, false otherwise  


## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
