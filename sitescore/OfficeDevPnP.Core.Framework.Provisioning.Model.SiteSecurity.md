# SiteSecurity Class
 Domain Object that is used in the site template   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel](OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel.md)  
## Syntax
```C#
public class SiteSecurity: BaseModel, IEquatable<SiteSecurity>
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [SiteSecurity()](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteSecurity.ctor1.md) | Constructor for SiteSecurity class 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [AdditionalAdministrators](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteSecurity.AdditionalAdministrators.md) | A Collection of users that are associated as site collection adminsitrators
| [AdditionalMembers](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteSecurity.AdditionalMembers.md) | A Collection of users that are associated to the sites members group
| [AdditionalOwners](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteSecurity.AdditionalOwners.md) | A Collection of users that are associated to the sites owners group
| [AdditionalVisitors](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteSecurity.AdditionalVisitors.md) | A Collection of users taht are associated to the sites visitors group
| [BreakRoleInheritance](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteSecurity.BreakRoleInheritance.md) | Declares whether the to break role inheritance for the site, if it is a sub-site
| [ClearSubscopes](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteSecurity.ClearSubscopes.md) | Defines whether to clear subscopes or not while breaking role inheritance for the site
| [CopyRoleAssignments](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteSecurity.CopyRoleAssignments.md) | Defines whether to copy role assignments or not while breaking role inheritance
| [SiteGroups](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteSecurity.SiteGroups.md) | List of additional Groups for the Site
| [SiteSecurityPermissions](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteSecurity.SiteSecurityPermissions.md) | List of Site Security Permissions for the Site
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Equals(Object)](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteSecurity.3520ddbb.md) | Compares object with SiteSecurity
| [Equals(SiteSecurity)](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteSecurity.98ba844a.md) | Compares SiteSecurity object based on AdditionalAdministrators, AdditionalOwners, AdditionalMembers, AdditionalVisitors, SiteGroups, SiteSecurityPermissions, BreakRoleInheritance, CopyRoleAssignments and ClearSubscopes properties.
| [GetHashCode()](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteSecurity.1c6872bd.md) | Gets the hash code
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
