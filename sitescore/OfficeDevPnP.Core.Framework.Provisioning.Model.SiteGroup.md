# SiteGroup Class
 The base type for a Site Group   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel](OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel.md)  
## Syntax
```C#
public class SiteGroup: BaseModel, IEquatable<SiteGroup>
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [SiteGroup()](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteGroup.ctor1.md) | Constructor for SiteGroup class 
| [SiteGroup(IEnumerable<User>)](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteGroup.ctor2.md) | Constructor for SiteGroup class 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [AllowMembersEditMembership](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteGroup.AllowMembersEditMembership.md) | Defines whether the members can edit membership of the Site Group
| [AllowRequestToJoinLeave](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteGroup.AllowRequestToJoinLeave.md) | Defines whether to allow requests to join or leave the Site Group
| [AutoAcceptRequestToJoinLeave](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteGroup.AutoAcceptRequestToJoinLeave.md) | Defines whether to auto-accept requests to join or leave the Site Group
| [Description](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteGroup.Description.md) | The Description of the Site Group
| [Members](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteGroup.Members.md) | The list of members of the Site Group
| [OnlyAllowMembersViewMembership](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteGroup.OnlyAllowMembersViewMembership.md) | Defines whether to allow members only to view the membership of the Site Group
| [Owner](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteGroup.Owner.md) | The Owner of the Site Group
| [RequestToJoinLeaveEmailSetting](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteGroup.RequestToJoinLeaveEmailSetting.md) | Defines the email address used for membership requests to join or leave will be sent for the Site Group
| [Title](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteGroup.Title.md) | The Title of the Site Group
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Equals(Object)](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteGroup.3520ddbb.md) | Compares object with SiteGroup
| [Equals(SiteGroup)](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteGroup.3ae0cc70.md) | Compares SiteGroup object based on AllowMembersEditMembership, AllowRequestToJoinLeave, AutoAcceptRequestToJoinLeave, Description, Members, OnlyAllowMembersViewMembership, Owner, RequestToJoinLeaveEmailSetting and Title properties.
| [GetHashCode()](OfficeDevPnP.Core.Framework.Provisioning.Model.SiteGroup.1c6872bd.md) | Gets the hash code
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
