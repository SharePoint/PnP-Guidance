# TaxonomyExtensions.ImportTerms Method  
 Imports an array of &brvbar; delimited strings into the deafult site collection termstore. Specify strings in this format: TermGroup&brvbar;TermSet&brvbar;Term E.g. "Locations&brvbar;Nordics&brvbar;Sweden"   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void ImportTerms(this Site site, String[] termLines, Int32 lcid, TermStore termStore, String delimiter = "|", Boolean synchronizeDeletions = False)
```
### Parameters
#### site  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Site  
&emsp;&emsp;The current site  

  

#### termLines  
&emsp;&emsp;Type: System.String[]  
&emsp;&emsp;Array of TermLines  

  

#### lcid  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Locale identifier (LCID) for the language  

  

#### termStore  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Taxonomy.TermStore  
&emsp;&emsp;The termstore to import the terms into  

  

#### (optional) delimiter  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;delimeter which seperates terms  

  

#### (optional) synchronizeDeletions  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Remove tags that are not present in the import  

  

### Return Value
Type: void  

## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
