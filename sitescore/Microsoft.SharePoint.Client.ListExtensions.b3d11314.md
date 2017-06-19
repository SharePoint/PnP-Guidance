# ListExtensions.GetDefaultColumnValues Method  


Gets default values for column values.



The returned list contains one dictionary per default setting per folder.

Each dictionary has the following keys set: Path, Field, Value



Path: Relative path to the library/folder

Field: Internal name of the field which has a default value

Value: The default value for the field  

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static List<Dictionary<String, String>> GetDefaultColumnValues(this List list)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;List to process  

  

### Return Value
Type: List<Dictionary<String,  String>>  

## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
