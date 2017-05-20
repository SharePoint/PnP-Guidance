# TaxonomyExtensions.EnsureTermGroup Method  
 Ensures the named group exists, returning a reference to the group, and creating or updating as necessary.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static TermGroup EnsureTermGroup(this Site site, String groupName, Guid groupId, String groupDescription)
```
### Parameters
#### site  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Site  
&emsp;&emsp;Site connected to the term store to use  

  

#### groupName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the term group  

  

#### (optional) groupId  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;(Optional) ID of the group; if not provided the parameter is ignored, a random GUID is used if necessary to create the group, otherwise if the ID differs a warning is logged  

  

#### (optional) groupDescription  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;(Optional) Description of the term group; if null or not provided the parameter is ignored, otherwise the group is updated as necessary to match the description; passing an empty string will clear the description  

  

### Return Value
Type: TermGroup  
The required term group  


## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
