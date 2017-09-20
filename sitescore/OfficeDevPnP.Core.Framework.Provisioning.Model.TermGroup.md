# TermGroup Class
  

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel](OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel.md)  
## Syntax
```C#
public class TermGroup: BaseModel, IEquatable<TermGroup>
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [TermGroup()](OfficeDevPnP.Core.Framework.Provisioning.Model.TermGroup.ctor1.md) | Constructor for TermGroup class 
| [TermGroup(Guid, String, List<TermSet>, Boolean, IEnumerable<User>, IEnumerable<User>)](OfficeDevPnP.Core.Framework.Provisioning.Model.TermGroup.ctor2.md) | Constructor for TermGroup class 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [Contributors](OfficeDevPnP.Core.Framework.Provisioning.Model.TermGroup.Contributors.md) | List of TermGroup Contributors
| [Description](OfficeDevPnP.Core.Framework.Provisioning.Model.TermGroup.Description.md) | The Description of the TermGroup
| [Id](OfficeDevPnP.Core.Framework.Provisioning.Model.TermGroup.Id.md) | The ID of the TermGroup
| [Managers](OfficeDevPnP.Core.Framework.Provisioning.Model.TermGroup.Managers.md) | List of TermGroup Managers
| [Name](OfficeDevPnP.Core.Framework.Provisioning.Model.TermGroup.Name.md) | The Name of the TermGroup
| [SiteCollectionTermGroup](OfficeDevPnP.Core.Framework.Provisioning.Model.TermGroup.SiteCollectionTermGroup.md) | Is this a site collection term group
| [TermSets](OfficeDevPnP.Core.Framework.Provisioning.Model.TermGroup.TermSets.md) | The collection of TermSet items in the TermGroup
| [UpdateBehavior](OfficeDevPnP.Core.Framework.Provisioning.Model.TermGroup.UpdateBehavior.md) | If the TermGroup already exists on target, this attribute defines whether the TermGroup will be overwritten or skipped.
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Equals(Object)](OfficeDevPnP.Core.Framework.Provisioning.Model.TermGroup.3520ddbb.md) | Compares object with TermGroup
| [Equals(TermGroup)](OfficeDevPnP.Core.Framework.Provisioning.Model.TermGroup.2061d3d1.md) | Compares TermGroup object based on Id, Name, Description and TermSets.
| [GetHashCode()](OfficeDevPnP.Core.Framework.Provisioning.Model.TermGroup.1c6872bd.md) | Gets the hash code
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
