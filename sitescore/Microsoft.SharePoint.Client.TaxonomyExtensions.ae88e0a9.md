# TaxonomyExtensions.CreateTermGroup Method  
 Creates a new term group, in the specified term store.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static TermGroup CreateTermGroup(this TermStore termStore, String groupName, Guid groupId, String groupDescription)
```
### Parameters
#### termStore  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Taxonomy.TermStore  
&emsp;&emsp;the term store to use  

  

#### groupName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the term group  

  

#### (optional) groupId  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;(Optional) ID of the group; if not provided a random GUID is used  

  

#### (optional) groupDescription  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;(Optional) Description of the term group  

  

### Return Value
Type: TermGroup  
The created term group  


## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
