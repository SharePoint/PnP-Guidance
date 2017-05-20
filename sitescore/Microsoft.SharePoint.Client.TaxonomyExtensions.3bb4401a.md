# TaxonomyExtensions.ImportTermSet Method  
 Imports terms from a term set file, updating with any new terms, in the same format at that used by the web interface import ability.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static TermSet ImportTermSet(this TermGroup termGroup, String filePath, Guid termSetId, Boolean synchroniseDeletions = False, Nullable<Boolean> termSetIsOpen, String termSetContact, String termSetOwner)
```
### Parameters
#### termGroup  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Taxonomy.TermGroup  
&emsp;&emsp;Group to create the term set within  

  

#### filePath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Local path to the file to import  

  

#### (optional) termSetId  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;GUID to use for the term set; if Guid.Empty is passed then a random GUID is generated and used  

  

#### (optional) synchroniseDeletions  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;(Optional) Whether to also synchronise deletions; that is, remove any terms not in the import file; default is no (false)  

  

#### (optional) termSetIsOpen  
&emsp;&emsp;Type: System.Nullable&lt;System.Boolean&gt;  
&emsp;&emsp;(Optional) Whether the term set should be marked open; if not passed, then the existing setting is not changed  

  

#### (optional) termSetContact  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;(Optional) Contact for the term set; if not provided, the existing setting is retained  

  

#### (optional) termSetOwner  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;(Optional) Owner for the term set; if not provided, the existing setting is retained  

  

### Return Value
Type: TermSet  
The created, or updated, term set  


## Remarks
 The format of the file is the same as that used by the import function in the web interface. A sample file can be obtained from the web interface. 
 This is a CSV file, with the following headings: 
Term Set Name,Term Set Description,LCID,Available for Tagging,Term Description,Level 1 Term,Level 2 Term,Level 3 Term,Level 4 Term,Level 5 Term,Level 6 Term,Level 7 Term
 The first data row must contain the Term Set Name, Term Set Description, and LCID, and should also contain the first term. 
 It is recommended that a fixed GUID be used as the termSetId, to allow the term set to be easily updated (so do not pass Guid.Empty). 
 In contrast to the web interface import, this is not a one-off import but runs synchronisation logic allowing updating of an existing Term Set. When synchronising, any existing terms are matched (with Term Description and Available for Tagging updated as necessary), any new terms are added in the correct place in the hierarchy, and (if synchroniseDeletions is set) any terms not in the imported file are removed. 
 The import file also supports an expanded syntax for the Term Set Name and term names (Level 1 Term, Level 2 Term, etc). These columns support values with the format "Name&brvbar;GUID", with the name and GUID separated by a pipe character (note that the pipe character is invalid to use within a taxomony item name). This expanded syntax is not required, but can be used to ensure all terms have fixed IDs. 
  
## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
