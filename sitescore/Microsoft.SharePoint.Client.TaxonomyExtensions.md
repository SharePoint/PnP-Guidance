# TaxonomyExtensions Class
 Class for deprecated taxonomy extension methods 

 Class for taxonomy extension methods   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class TaxonomyExtensions
```
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [DenormalizeName(String)](Microsoft.SharePoint.Client.TaxonomyExtensions.fce4464c.md) | Denormalizes a Taxonomy name
| [NormalizeName(String)](Microsoft.SharePoint.Client.TaxonomyExtensions.980773b1.md) | Normalizes a Taxonomy name
## Extension Methods
|**Name**|**Description**|
|:-----|:-----|
| [AddTermToTermset(Site, Guid, String)](Microsoft.SharePoint.Client.TaxonomyExtensions.8c1fbbaf.md) | Adds a term to a given termset
| [AddTermToTermset(Site, Guid, String, Guid)](Microsoft.SharePoint.Client.TaxonomyExtensions.3589b8ac.md) | Adds a term to a given termset
| [CreateTaxonomyField(Web, TaxonomyFieldCreationInformation)](Microsoft.SharePoint.Client.TaxonomyExtensions.6008c17a.md) | Can be used to create taxonomy field remotely to web.
| [CreateTaxonomyField(List, TaxonomyFieldCreationInformation)](Microsoft.SharePoint.Client.TaxonomyExtensions.61031b4.md) | Can be used to create taxonomy field remotely in a list.
| [CreateTermGroup(TermStore, String, Guid, String)](Microsoft.SharePoint.Client.TaxonomyExtensions.ae88e0a9.md) | Creates a new term group, in the specified term store.
| [EnsureTermGroup(Site, String, Guid, String)](Microsoft.SharePoint.Client.TaxonomyExtensions.8773c292.md) | Ensures the named group exists, returning a reference to the group, and creating or updating as necessary.
| [EnsureTermSet(TermGroup, String, Guid, Nullable&lt;Int32&gt;, String, Nullable&lt;Boolean&gt;, String, String)](Microsoft.SharePoint.Client.TaxonomyExtensions.de7dfc70.md) | Ensures the named term set exists, returning a reference to the set, and creating or updating as necessary.
| [ExportAllTerms(Site, Boolean, String)](Microsoft.SharePoint.Client.TaxonomyExtensions.eb0ebf3c.md) | Exports the full list of terms from all termsets in all termstores.
| [ExportTermSet(Site, Guid, Boolean, String)](Microsoft.SharePoint.Client.TaxonomyExtensions.a25b0591.md) | Exports the full list of terms from all termsets in all termstores.
| [ExportTermSet(Site, Guid, Boolean, TermStore, String)](Microsoft.SharePoint.Client.TaxonomyExtensions.ecbde79a.md) | Exports the full list of terms from all termsets in all termstores.
| [GetDefaultKeywordsTermStore(Site)](Microsoft.SharePoint.Client.TaxonomyExtensions.88b3540.md) | Returns the default keywords termstore for the current site
| [GetDefaultSiteCollectionTermStore(Site)](Microsoft.SharePoint.Client.TaxonomyExtensions.dace4ac5.md) | Returns the default site collection termstore
| [GetTaxonomyItemByPath(Site, String, String)](Microsoft.SharePoint.Client.TaxonomyExtensions.c526145c.md) | Returns a taxonomy item by it's path, e.g. Group&brvbar;Set&brvbar;Term
| [GetTaxonomySession(Site)](Microsoft.SharePoint.Client.TaxonomyExtensions.a8117943.md) | Returns a new taxonomy session for the current site
| [GetTermByName(Site, Guid, String)](Microsoft.SharePoint.Client.TaxonomyExtensions.950b00c9.md) | Gets a Taxonomy Term by Name
| [GetTermGroupById(Site, Guid)](Microsoft.SharePoint.Client.TaxonomyExtensions.3cd146f5.md) | Finds a termgroup by its ID
| [GetTermGroupByName(Site, String)](Microsoft.SharePoint.Client.TaxonomyExtensions.e33279e7.md) | Finds a termgroup by name
| [GetTermGroupByName(TermStore, String)](Microsoft.SharePoint.Client.TaxonomyExtensions.f08e91ac.md) | Gets the named term group, if it exists in the term store.
| [GetTermSetsByName(Site, String, Int32)](Microsoft.SharePoint.Client.TaxonomyExtensions.cb9a8e23.md) | Finds a termset by name
| [GetWssIdForTerm(Web, Term)](Microsoft.SharePoint.Client.TaxonomyExtensions.32328193.md) | Returns the Id for a term if present in the TaxonomyHiddenList. Otherwise returns -1;
| [ImportTerms(Site, String[], Int32, String, Boolean)](Microsoft.SharePoint.Client.TaxonomyExtensions.767ce9a0.md) | Imports an array of &brvbar; delimited strings into the deafult site collection termstore. Specify strings in this format: TermGroup&brvbar;TermSet&brvbar;Term E.g. "Locations&brvbar;Nordics&brvbar;Sweden"
| [ImportTerms(Site, String[], Int32, TermStore, String, Boolean)](Microsoft.SharePoint.Client.TaxonomyExtensions.dcedec05.md) | Imports an array of &brvbar; delimited strings into the deafult site collection termstore. Specify strings in this format: TermGroup&brvbar;TermSet&brvbar;Term E.g. "Locations&brvbar;Nordics&brvbar;Sweden"
| [ImportTermSet(TermGroup, String, Guid, Boolean, Nullable&lt;Boolean&gt;, String, String)](Microsoft.SharePoint.Client.TaxonomyExtensions.3bb4401a.md) | Imports terms from a term set file, updating with any new terms, in the same format at that used by the web interface import ability.
| [ImportTermSet(TermGroup, Stream, Guid, Boolean, Nullable&lt;Boolean&gt;, String, String)](Microsoft.SharePoint.Client.TaxonomyExtensions.dea02e42.md) | Imports terms from a term set stream, updating with any new terms, in the same format at that used by the web interface import ability.
| [RemoveTaxonomyFieldById(Web, Guid)](Microsoft.SharePoint.Client.TaxonomyExtensions.20d5705f.md) | Removes a taxonomy field (site column) and its associated hidden field by id
| [RemoveTaxonomyFieldByInternalName(Web, String)](Microsoft.SharePoint.Client.TaxonomyExtensions.9f4bb750.md) | Removes a taxonomy field (site column) and its associated hidden field by internal name
| [SetTaxonomyFieldDefaultValue(Field, TaxonomyItem, String, Boolean)](Microsoft.SharePoint.Client.TaxonomyExtensions.8f744f2e.md) | Sets the default value for a managed metadata field
| [SetTaxonomyFieldValue(ListItem, Guid, String, Guid)](Microsoft.SharePoint.Client.TaxonomyExtensions.f79bdcab.md) | Sets a value of a taxonomy field
| [SetTaxonomyFieldValueByTermPath(ListItem, String, Guid)](Microsoft.SharePoint.Client.TaxonomyExtensions.5a80eb78.md) | Sets a value in a taxonomy field
| [SetTaxonomyFieldValues(ListItem, Guid, IEnumerable&lt;KeyValuePair&lt;Guid, String&gt;&gt;)](Microsoft.SharePoint.Client.TaxonomyExtensions.927e70c0.md) | Sets a value of a taxonomy field that supports multiple values
| [WireUpTaxonomyField(Web, Field, String, String, Boolean)](Microsoft.SharePoint.Client.TaxonomyExtensions.298466cf.md) | Wires up MMS field to the specified term set.
| [WireUpTaxonomyField(Web, Field, TermSet, Boolean)](Microsoft.SharePoint.Client.TaxonomyExtensions.f35778b0.md) | Wires up MMS field to the specified term set.
| [WireUpTaxonomyField(Web, Field, Term, Boolean)](Microsoft.SharePoint.Client.TaxonomyExtensions.a589d5c2.md) | Wires up MMS field to the specified term.
| [WireUpTaxonomyField(Web, Guid, String, String, Boolean)](Microsoft.SharePoint.Client.TaxonomyExtensions.c812b6c0.md) | Wires up MMS field to the specified term set.
| [WireUpTaxonomyField(List, Field, TermSet, Boolean)](Microsoft.SharePoint.Client.TaxonomyExtensions.1a55b0c7.md) | Wires up MMS field to the specified term set.
| [WireUpTaxonomyField(List, Field, Term, Boolean)](Microsoft.SharePoint.Client.TaxonomyExtensions.5a4045b7.md) | Wires up MMS field to the specified term.
| [WireUpTaxonomyField(List, Field, String, String, Boolean)](Microsoft.SharePoint.Client.TaxonomyExtensions.985cc78b.md) | Wires up MMS field to the specified term set.
| [WireUpTaxonomyField(List, Guid, String, String, Boolean)](Microsoft.SharePoint.Client.TaxonomyExtensions.a5f7f2d0.md) | Wires up MMS field to the specified term set.
## See also
- System.Collections.Generic.KeyNotFoundException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)
