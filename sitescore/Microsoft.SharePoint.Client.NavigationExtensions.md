# NavigationExtensions Class
 This class holds deprecated navigation related methods 

 This class holds navigation related methods   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class NavigationExtensions
```
## Extension Methods
|**Name**|**Description**|
|:-----|:-----|
| [AddCustomAction(Web, CustomActionEntity)](Microsoft.SharePoint.Client.NavigationExtensions.c58ae7f0.md) | Adds custom action to a web. If the CustomAction exists the item will be updated. Setting CustomActionEntity.Remove == true will delete the CustomAction.
| [AddCustomAction(Site, CustomActionEntity)](Microsoft.SharePoint.Client.NavigationExtensions.c238735d.md) | Adds custom action to a site collection. If the CustomAction exists the item will be updated. Setting CustomActionEntity.Remove == true will delete the CustomAction.
| [AddNavigationNode(Web, String, Uri, String, NavigationType, Boolean, Boolean)](Microsoft.SharePoint.Client.NavigationExtensions.379f276c.md) | Add a node to quick launch, top navigation bar or search navigation. The node will be added as the last node in the collection.
| [CustomActionExists(Web, String)](Microsoft.SharePoint.Client.NavigationExtensions.45893840.md) | Utility method to check particular custom action already exists on the web
| [CustomActionExists(Site, String)](Microsoft.SharePoint.Client.NavigationExtensions.d520d62a.md) | Utility method to check particular custom action already exists on the web
| [DeleteAllNavigationNodes(Web, NavigationType)](Microsoft.SharePoint.Client.NavigationExtensions.bfcb26ce.md) | Deletes all Navigation Nodes from a given navigation
| [DeleteCustomAction(Web, Guid)](Microsoft.SharePoint.Client.NavigationExtensions.4bb46a7f.md) | Removes a custom action
| [DeleteCustomAction(Site, Guid)](Microsoft.SharePoint.Client.NavigationExtensions.f2016670.md) | Removes a custom action
| [DeleteNavigationNode(Web, String, String, NavigationType)](Microsoft.SharePoint.Client.NavigationExtensions.54c91f2e.md) | Deletes a navigation node from the quickLaunch or top navigation bar
| [GetCustomActions(Web, Expression&lt;Func&lt;UserCustomAction, Object&gt;&gt;[])](Microsoft.SharePoint.Client.NavigationExtensions.eac0e89b.md) | Returns all custom actions in a web
| [GetCustomActions(Site, Expression&lt;Func&lt;UserCustomAction, Object&gt;&gt;[])](Microsoft.SharePoint.Client.NavigationExtensions.fc5b2546.md) | Returns all custom actions in a web
| [GetEditableNavigationTermSet(Web, ManagedNavigationKind)](Microsoft.SharePoint.Client.NavigationExtensions.12efa587.md) | Returns an editable version of the Global Navigation TermSet for a web site
| [GetNavigationSettings(Web)](Microsoft.SharePoint.Client.NavigationExtensions.c72dbb5.md) | Returns the navigation settings for the selected web
| [IsManagedNavigationEnabled(Web, ManagedNavigationKind)](Microsoft.SharePoint.Client.NavigationExtensions.60d1127.md) | Determines whether the current Web has the managed navigation enabled
| [LoadSearchNavigation(Web)](Microsoft.SharePoint.Client.NavigationExtensions.4bb1e553.md) | Loads the search navigation nodes
| [UpdateNavigationInheritance(Web, Boolean)](Microsoft.SharePoint.Client.NavigationExtensions.c7232652.md) | Updates the navigation inheritance setting
| [UpdateNavigationSettings(Web, AreaNavigationEntity)](Microsoft.SharePoint.Client.NavigationExtensions.419cdf55.md) | Updates navigation settings for the current web
## Examples
```C#
var editAction = new CustomActionEntity()
{
   Title = "Edit Site Classification",
   Description = "Manage business impact information for site collection or sub sites.",
   Sequence = 1000,
   Group = "SiteActions",
   Location = "Microsoft.SharePoint.StandardMenu",
   Url = EditFormUrl,
   ImageUrl = EditFormImageUrl,
   Rights = new BasePermissions(),
};
editAction.Rights.Set(PermissionKind.ManageWeb);
web.AddCustomAction(editAction);
```

## See also
- GetCustomActions
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)
