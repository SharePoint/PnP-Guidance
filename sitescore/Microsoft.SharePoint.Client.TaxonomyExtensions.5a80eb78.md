# TaxonomyExtensions.SetTaxonomyFieldValueByTermPath Method  
 Sets a value in a taxonomy field   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetTaxonomyFieldValueByTermPath(this ListItem item, String TermPath, Guid fieldId)
```
### Parameters
#### item  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ListItem  
&emsp;&emsp;The item to set the value to  

  

#### TermPath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The path of the term in the shape of "TermGroupName|TermSetName|TermName"  

  

#### fieldId  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;The id of the field  

  

### Return Value
Type: void  

## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- System.Collections.Generic.KeyNotFoundException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
