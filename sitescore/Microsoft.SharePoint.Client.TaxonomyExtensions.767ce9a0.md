# TaxonomyExtensions.ImportTerms Method  
 Imports an array of &brvbar; delimited strings into the deafult site collection termstore. Specify strings in this format: TermGroup&brvbar;TermSet&brvbar;Term E.g. "Locations&brvbar;Nordics&brvbar;Sweden"   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void ImportTerms(Site site, String[] termLines, Int32 lcid, String delimiter, Boolean synchronizeDeletions)
```
### Parameters
#### site  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Site  
&emsp;&emsp; Imports an array of &brvbar; delimited strings into the deafult site collection termstore. Specify strings in this format: TermGroup&brvbar;TermSet&brvbar;Term E.g. "Locations&brvbar;Nordics&brvbar;Sweden"   

  

#### termLines  
&emsp;&emsp;Type: System.String[]  
&emsp;&emsp; Imports an array of &brvbar; delimited strings into the deafult site collection termstore. Specify strings in this format: TermGroup&brvbar;TermSet&brvbar;Term E.g. "Locations&brvbar;Nordics&brvbar;Sweden"   

  

#### lcid  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp; Imports an array of &brvbar; delimited strings into the deafult site collection termstore. Specify strings in this format: TermGroup&brvbar;TermSet&brvbar;Term E.g. "Locations&brvbar;Nordics&brvbar;Sweden"   

  

#### (optional) delimiter  
&emsp;&emsp;Type: System.String  
&emsp;&emsp; Imports an array of &brvbar; delimited strings into the deafult site collection termstore. Specify strings in this format: TermGroup&brvbar;TermSet&brvbar;Term E.g. "Locations&brvbar;Nordics&brvbar;Sweden"   

  

#### (optional) synchronizeDeletions  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Remove tags that are not present in the import  

  

### Return Value
Type: void  

## Remarks
  
## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
