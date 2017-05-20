# TaxonomyExtensions.SetTaxonomyFieldValues Method  
 Sets a value of a taxonomy field that supports multiple values   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetTaxonomyFieldValues(this ListItem item, Guid fieldId, IEnumerable<KeyValuePair<Guid, String>> termValues)
```
### Parameters
#### item  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ListItem  
&emsp;&emsp;The item to process  

  

#### fieldId  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;The ID of the field to set  

  

#### termValues  
&emsp;&emsp;Type: System.Collections.Generic.IEnumerable&lt;System.Collections.Generic.KeyValuePair&lt;System.Guid, System.String&gt;&gt;  
&emsp;&emsp;The key and values of terms to set  

  

### Return Value
Type: void  

## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
