# TaxonomyExtensions.WireUpTaxonomyField Method  
 Wires up MMS field to the specified term.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void WireUpTaxonomyField(this List list, Field field, Term anchorTerm, Boolean multiValue = False)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;List to be processed  

  

#### field  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Field  
&emsp;&emsp;Field to be wired up  

  

#### anchorTerm  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Taxonomy.Term  
&emsp;&emsp;Taxonomy Term  

  

#### (optional) multiValue  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Allow multiple selection  

  

### Return Value
Type: void  

## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
