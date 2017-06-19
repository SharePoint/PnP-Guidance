# TaxonomyExtensions.GetTermSetsByName Method  
 Finds a termset by name   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static TermSetCollection GetTermSetsByName(this Site site, String name, Int32 lcid = 1033)
```
### Parameters
#### site  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Site  
&emsp;&emsp;The current site  

  

#### name  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The name of the termset  

  

#### (optional) lcid  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;The locale ID for the termset to return, defaults to 1033  

  

### Return Value
Type: TermSetCollection  
Returns collection of TermSet  


## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
