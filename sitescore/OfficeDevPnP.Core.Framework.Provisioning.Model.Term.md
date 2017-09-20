# Term Class
  

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel](OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel.md)  
## Syntax
```C#
public class Term: BaseModel, IEquatable<Term>
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [Term()](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.ctor1.md) | Constructor for Term class 
| [Term(Guid, String, Nullable<Int32>, List<Term>, List<TermLabel>, Dictionary<String, String>, Dictionary<String, String>)](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.ctor2.md) | Constructor for Term class 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [CustomSortOrder](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.CustomSortOrder.md) | Gets or sets the order of the term
| [Description](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.Description.md) | Gets or sets the term description
| [Id](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.Id.md) | Gets or sets the term id
| [IsAvailableForTagging](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.IsAvailableForTagging.md) | Gets or sets the IsAvailableForTagging flag for the term
| [IsDeprecated](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.IsDeprecated.md) | Gets or sets the IsDeprecated flag for the term
| [IsReused](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.IsReused.md) | Gets or sets the IsReused flag for the term
| [IsSourceTerm](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.IsSourceTerm.md) | Gets or sets the IsSourceTerm flag for the term
| [Labels](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.Labels.md) | Gets or sets term labels
| [Language](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.Language.md) | Gets or sets Language of the term
| [LocalProperties](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.LocalProperties.md) | Gets or sets local properties for the term
| [Name](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.Name.md) | Gets or sets the term name
| [Owner](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.Owner.md) | Gets or sets the term owner
| [Properties](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.Properties.md) | Gets or sets the properties of the term
| [SourceTermId](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.SourceTermId.md) | Gets or sets the term source id
| [Terms](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.Terms.md) | Gets or sets terms
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Equals(Object)](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.3520ddbb.md) | Compares object with Term
| [Equals(Term)](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.456809bc.md) | Compares Term object based on Id, Name, Description, Language, Owner, IsAvailableForTagging, IsReused, IsSourceTerm, SourceTermId, IsDeprecated, CustomSortOrder, Labels, Terms, Properties and LocalProperties.
| [GetHashCode()](OfficeDevPnP.Core.Framework.Provisioning.Model.Term.1c6872bd.md) | Gets the hash code
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
