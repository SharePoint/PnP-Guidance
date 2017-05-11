# TaxonomyExtensions.SetTaxonomyFieldValues Method  
 Sets a value of a taxonomy field that supports multiple values   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetTaxonomyFieldValues(ListItem item, Guid fieldId, IEnumerable<KeyValuePair<Guid, String>> termValues)
```
### Parameters
#### item  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ListItem  
&emsp;&emsp;The item to process  

  

#### fieldId  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;The ID of the field to set  

  

#### termValues  
&emsp;&emsp;Type: System.Collections.Generic.IEnumerable<System.Collections.Generic.KeyValuePair<System.Guid, System.String>>  
&emsp;&emsp;The key and values of terms to set  

  

### Return Value
Type: void  

## Remarks
  
## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
