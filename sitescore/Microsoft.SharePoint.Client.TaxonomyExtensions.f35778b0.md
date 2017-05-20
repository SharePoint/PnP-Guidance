# TaxonomyExtensions.WireUpTaxonomyField Method  
 Wires up MMS field to the specified term set.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void WireUpTaxonomyField(this Web web, Field field, TermSet termSet, Boolean multiValue = False)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### field  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Field  
&emsp;&emsp;Field to be wired up  

  

#### termSet  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Taxonomy.TermSet  
&emsp;&emsp;Taxonomy TermSet  

  

#### (optional) multiValue  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;If true, create a multivalue field  

  

### Return Value
Type: void  

## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
