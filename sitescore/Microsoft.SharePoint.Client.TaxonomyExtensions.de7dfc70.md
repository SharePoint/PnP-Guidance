# TaxonomyExtensions.EnsureTermSet Method  
 Ensures the named term set exists, returning a reference to the set, and creating or updating as necessary.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static TermSet EnsureTermSet(this TermGroup parentGroup, String termSetName, Guid termSetId, Nullable<Int32> lcid, String description, Nullable<Boolean> isOpen, String termSetContact, String termSetOwner)
```
### Parameters
#### parentGroup  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Taxonomy.TermGroup  
&emsp;&emsp;Group to check or create the term set in  

  

#### termSetName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the term set  

  

#### (optional) termSetId  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;(Optional) ID of the term set; if not provided the parameter is ignored, a random GUID is used if necessary to create the term set, otherwise if the ID differs a warning is logged  

  

#### (optional) lcid  
&emsp;&emsp;Type: System.Nullable&lt;System.Int32&gt;  
&emsp;&emsp;(Optional) Default language of the term set; if not provided the default of the associate term store is used  

  

#### (optional) description  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;(Optional) Description of the term set; if null or not provided the parameter is ignored, otherwise the term set is updated as necessary to match the description; passing an empty string will clear the description  

  

#### (optional) isOpen  
&emsp;&emsp;Type: System.Nullable&lt;System.Boolean&gt;  
&emsp;&emsp;(Optional) Whether the term store is open for new term creation or not  

  

#### (optional) termSetContact  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;(Optional) E-mail address for term suggestions and feedback  

  

#### (optional) termSetOwner  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Owner of termset  

  

### Return Value
Type: TermSet  
The required term set  


## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
