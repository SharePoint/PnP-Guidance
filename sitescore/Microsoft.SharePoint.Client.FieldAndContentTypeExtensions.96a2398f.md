# FieldAndContentTypeExtensions.GetFields Method  
 Gets a list of fields from a list by names.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static IEnumerable<Field> GetFields(this List list, params String[] fieldInternalNames)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;The target list containing the fields.  

  

#### fieldInternalNames  
&emsp;&emsp;Type: System.String[]  
&emsp;&emsp;List of field names to retreieve.  

  

### Return Value
Type: IEnumerable<Field>  
List of fields requested.  


## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
