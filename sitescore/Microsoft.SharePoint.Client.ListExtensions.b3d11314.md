# ListExtensions.GetDefaultColumnValues Method  
 &lt;para&gt;Gets default values for column values.&lt;/para&gt; &lt;para&gt;&lt;/para&gt; &lt;para&gt;The returned list contains one dictionary per default setting per folder.&lt;/para&gt; &lt;para&gt;Each dictionary has the following keys set: Path, Field, Value&lt;/para&gt; &lt;para&gt;&lt;/para&gt; &lt;para&gt;Path: Relative path to the library/folder&lt;/para&gt; &lt;para&gt;Field: Internal name of the field which has a default value&lt;/para&gt; &lt;para&gt;Value: The default value for the field&lt;/para&gt;   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static List<Dictionary<String, String>> GetDefaultColumnValues(List list)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp; &lt;para&gt;Gets default values for column values.&lt;/para&gt; &lt;para&gt;&lt;/para&gt; &lt;para&gt;The returned list contains one dictionary per default setting per folder.&lt;/para&gt; &lt;para&gt;Each dictionary has the following keys set: Path, Field, Value&lt;/para&gt; &lt;para&gt;&lt;/para&gt; &lt;para&gt;Path: Relative path to the library/folder&lt;/para&gt; &lt;para&gt;Field: Internal name of the field which has a default value&lt;/para&gt; &lt;para&gt;Value: The default value for the field&lt;/para&gt;   

  

### Return Value
Type: List<Dictionary<String,  String>>  

## Remarks
  
## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
