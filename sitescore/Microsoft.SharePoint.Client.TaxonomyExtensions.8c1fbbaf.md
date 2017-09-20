# TaxonomyExtensions.AddTermToTermset Method  
 Adds a term to a given termset   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Term AddTermToTermset(this Site site, Guid termSetId, String term)
```
### Parameters
#### site  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Site  
&emsp;&emsp;The current site  

  

#### termSetId  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;The ID of the termset  

  

#### term  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The label of the new term to create  

  

### Return Value
Type: Term  
Returns Term object  


## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
