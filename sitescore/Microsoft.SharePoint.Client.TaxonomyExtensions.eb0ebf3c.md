# TaxonomyExtensions.ExportAllTerms Method  
 Exports the full list of terms from all termsets in all termstores.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static List<String> ExportAllTerms(this Site site, Boolean includeId, String delimiter = "|")
```
### Parameters
#### site  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Site  
&emsp;&emsp;The site to process  

  

#### includeId  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;if true, Ids of the the taxonomy items will be included  

  

#### (optional) delimiter  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;if specified, this delimiter will be used. Notice that IDs will be delimited with ;# from the label  

  

### Return Value
Type: List<String>  
Returns list of Term strings  


## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
