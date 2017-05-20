# TaxonomyExtensions.SetTaxonomyFieldValue Method  
 Sets a value of a taxonomy field   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetTaxonomyFieldValue(this ListItem item, Guid fieldId, String label, Guid termGuid)
```
### Parameters
#### item  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ListItem  
&emsp;&emsp;The item to process  

  

#### fieldId  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;The ID of the field to set  

  

#### label  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The label of the term to set  

  

#### termGuid  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;The id of the term to set  

  

### Return Value
Type: void  

## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
