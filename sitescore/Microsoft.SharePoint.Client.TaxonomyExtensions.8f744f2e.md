# TaxonomyExtensions.SetTaxonomyFieldDefaultValue Method  
 Sets the default value for a managed metadata field   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetTaxonomyFieldDefaultValue(this Field field, TaxonomyItem taxonomyItem, String defaultValue, Boolean pushChangesToLists = False)
```
### Parameters
#### field  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Field  
&emsp;&emsp;Field to be wired up  

  

#### taxonomyItem  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Taxonomy.TaxonomyItem  
&emsp;&emsp;Taxonomy TermSet or Term  

  

#### defaultValue  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;default value for the field  

  

#### (optional) pushChangesToLists  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;push changes to lists  

  

### Return Value
Type: void  

## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
