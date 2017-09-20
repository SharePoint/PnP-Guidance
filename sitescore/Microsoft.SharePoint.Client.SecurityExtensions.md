# SecurityExtensions Class
 This manager class holds deprecated security related methods 

 This manager class holds security related methods   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class SecurityExtensions
```
## Extension Methods
|**Name**|**Description**|
|:-----|:-----|
| [AddAdministrators(Web, List&lt;UserEntity&gt;, Boolean)](Microsoft.SharePoint.Client.SecurityExtensions.6ae7b819.md) | Add a site collection administrator to a site collection
| [AddGroup(Web, String, String, Boolean, Boolean, Boolean)](Microsoft.SharePoint.Client.SecurityExtensions.6821c296.md) | Adds a group
| [AddPermissionLevelToGroup(SecurableObject, String, RoleType, Boolean)](Microsoft.SharePoint.Client.SecurityExtensions.7e8844c.md) | Add a permission level (e.g.Contribute, Reader,...) to a group
| [AddPermissionLevelToGroup(SecurableObject, String, String, Boolean)](Microsoft.SharePoint.Client.SecurityExtensions.e4482cf4.md) | Add a role definition (e.g.Contribute, Read, Approve) to a group
| [AddPermissionLevelToPrincipal(SecurableObject, Principal, RoleType, Boolean)](Microsoft.SharePoint.Client.SecurityExtensions.27dd60bf.md) | Add a permission level (e.g.Contribute, Reader,...) to a group
| [AddPermissionLevelToPrincipal(SecurableObject, Principal, String, Boolean)](Microsoft.SharePoint.Client.SecurityExtensions.bcafbed3.md) | Add a role definition (e.g.Contribute, Read, Approve) to a group
| [AddPermissionLevelToUser(SecurableObject, String, RoleType, Boolean)](Microsoft.SharePoint.Client.SecurityExtensions.5adad6c1.md) | Add a permission level (e.g.Contribute, Reader,...) to a user
| [AddPermissionLevelToUser(SecurableObject, String, String, Boolean)](Microsoft.SharePoint.Client.SecurityExtensions.f973c234.md) | Add a role definition (e.g.Contribute, Read, Approve) to a user
| [AddReaderAccess(Web)](Microsoft.SharePoint.Client.SecurityExtensions.ed280cd0.md) | Add read access to the group "Everyone except external users".
| [AddReaderAccess(Web, BuiltInIdentity)](Microsoft.SharePoint.Client.SecurityExtensions.c7da83a8.md) | Add read access to the group "Everyone except external users".
| [AddUserToGroup(Web, String, String)](Microsoft.SharePoint.Client.SecurityExtensions.174da59d.md) | Adds a user to a group
| [AddUserToGroup(Web, Int32, String)](Microsoft.SharePoint.Client.SecurityExtensions.a15d4933.md) | Adds a user to a group
| [AddUserToGroup(Web, Group, User)](Microsoft.SharePoint.Client.SecurityExtensions.86e5291a.md) | Adds a user to a group
| [AddUserToGroup(Web, Group, String)](Microsoft.SharePoint.Client.SecurityExtensions.fb8dc920.md) | Adds a user to a group
| [AssociateDefaultGroups(Web, Group, Group, Group)](Microsoft.SharePoint.Client.SecurityExtensions.9ceaf057.md) | Associate the provided groups as default owners, members or visitors groups. If a group is null then the association is not done
| [GetAdministrators(Web)](Microsoft.SharePoint.Client.SecurityExtensions.10b24275.md) | Get a list of site collection administrators
| [GetAllUniqueRoleAssignments(Web, Int32)](Microsoft.SharePoint.Client.SecurityExtensions.daa2e7f4.md) | Get all unique role assignments for a web object and all its descendents down to document or list item level.
| [GetAuthenticationRealm(Web)](Microsoft.SharePoint.Client.SecurityExtensions.c7f71f9e.md) | Returns the authentication realm for the current web
| [GetExternalUsersForSiteTenant(Web, Uri)](Microsoft.SharePoint.Client.SecurityExtensions.96e5dabd.md) | Returns a list all external users for a given site that have at least the viewpages permission
| [GetExternalUsersTenant(Web)](Microsoft.SharePoint.Client.SecurityExtensions.dac3008a.md) | Returns a list all external users in your tenant
| [GetGroupID(Web, String)](Microsoft.SharePoint.Client.SecurityExtensions.14a0cf4f.md) | Returns the integer ID for a given group name
| [GetSharingCapabilitiesTenant(Web, Uri)](Microsoft.SharePoint.Client.SecurityExtensions.6165887c.md) | Get the external sharing settings for the provided site. Only works in Office 365 Multi-Tenant
| [GroupExists(Web, String)](Microsoft.SharePoint.Client.SecurityExtensions.7e0748a8.md) | Checks if a group exists
| [IsUserInGroup(Web, String, String)](Microsoft.SharePoint.Client.SecurityExtensions.75d377f2.md) | Checks if a user is member of a group
| [RemoveAdministrator(Web, UserEntity)](Microsoft.SharePoint.Client.SecurityExtensions.fe945eb0.md) | Removes an administrators from the site collection
| [RemoveGroup(Web, String)](Microsoft.SharePoint.Client.SecurityExtensions.20a8af35.md) | Remove a group
| [RemoveGroup(Web, Group)](Microsoft.SharePoint.Client.SecurityExtensions.bfa1ee44.md) | Remove a group
| [RemovePermissionLevelFromGroup(SecurableObject, String, RoleType, Boolean)](Microsoft.SharePoint.Client.SecurityExtensions.d42b6c97.md) | Removes a permission level from a group
| [RemovePermissionLevelFromGroup(SecurableObject, String, String, Boolean)](Microsoft.SharePoint.Client.SecurityExtensions.64eef5df.md) | Removes a permission level from a group
| [RemovePermissionLevelFromPrincipal(SecurableObject, Principal, RoleType, Boolean)](Microsoft.SharePoint.Client.SecurityExtensions.8f162e10.md) | Removes a permission level from a user
| [RemovePermissionLevelFromPrincipal(SecurableObject, Principal, String, Boolean)](Microsoft.SharePoint.Client.SecurityExtensions.f3f34f1.md) | Removes a permission level from a user
| [RemovePermissionLevelFromUser(SecurableObject, String, RoleType, Boolean)](Microsoft.SharePoint.Client.SecurityExtensions.b4db0942.md) | Removes a permission level from a user
| [RemovePermissionLevelFromUser(SecurableObject, String, String, Boolean)](Microsoft.SharePoint.Client.SecurityExtensions.4d6b82ef.md) | Removes a permission level from a user
| [RemoveUserFromGroup(Web, String, String)](Microsoft.SharePoint.Client.SecurityExtensions.ec40d40c.md) | Removes a user from a group
| [RemoveUserFromGroup(Web, Group, User)](Microsoft.SharePoint.Client.SecurityExtensions.138472c.md) | Removes a user from a group
## See also
- [OfficeDevPnP.Core.Entities.UserEntity](OfficeDevPnP.Core.Entities.UserEntity.md)
- [OfficeDevPnP.Core.Entities.ExternalUserEntity](OfficeDevPnP.Core.Entities.ExternalUserEntity.md)
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)
