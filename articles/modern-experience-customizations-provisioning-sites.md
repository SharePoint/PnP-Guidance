# Provisioning modern team sites programmatically
Take a look on the options around provisioning modern team sites in SharePoint Online. Modern team sites have been introduced in SharePoint Online during autumn 2016 and usage of them can be controlled on tenant level. This article explains different options and considerations to create modern team sites in SharePoint Online. 

_**Applies to:** SharePoint Online_

## Provisioning a modern team site from user interface
<a name="sectionSection0"> </a>
There are numerous routes for a modern team site to get provisioned. You can start the provisioning directly from the SharePoint Online side or alternatively provision a Office 365 group for other locations, which will also provision a modern team site. 
- If modern team sites are enabled in SharePoit Online admin side, you can create modern team sites from the SharePoint home page
- You can create Office 365 group from the Office 365 Outlook and when you access the 'site' tab of a group, you will land on modern team site 

### How to control default provisioning flow
You can control SharePoint site creation process from the SharePoint Online admin settings. You can control if the modern experience is available for the end users or if you'd like to keep on using the classic experience.

![Site Creation options from the SharePoint Online admin UI](media/modern-experiences/site-creation-options-admin-ui.png)

See following Office Support article for details
- Manage site creation in SharePoint Online: https://support.office.com/en-US/article/Manage-site-creation-in-SharePoint-Online-e72844a3-0171-47c9-befb-e98b23e2dcf9

## Provisioning a modern team site programmatically
<a name="sectionSection0"> </a>
Modern team sites are created programmatically by creating a [Office 365 group](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/resources/group) using Microsoft Graph. When you create a Office 365 group a modern team site is automatically provisioned for the group and well. Modern team site URI will be taken from the mailNickname parameter of the Office 365 group and has following default structure. 

```
https://[tenant].sharepoint.com/sites/[mailNickname]]
``` 

> Detailed description group creation using Microsoft Graph is available from the [official documentation](https://graph.microsoft.io/en-us/docs/api-reference/v1.0/api/group_post_groups).

### Provisioning a modern team site with PnP CSOM core component
<a name="sectionSection0"> </a>
PnP CSOM Core component, available as a [NuGet package](https://www.nuget.org/packages/SharePointPnPCoreOnline), has simplified methods for the modern group handling. 

```C#
/// <summary>
/// Let's use UnifiedGroupsUtility class from PnP CSOM Core to simplify managed code operations with Office 365 groups
/// </summary>
/// <param name="accessToken">Azure AD Access token with Group.ReadWrite.All permission</param>
public static void ManipulateModernTeamSite(string accessToken)
{
    // Create new modern team site to url https://[tenant].sharepoint.com/sites/mymodernteamsite
    Stream groupLogoStream = new FileStream("C:\\groupassets\\logo-original.png", 
                                            FileMode.Open, FileAccess.Read);
    var group = UnifiedGroupsUtility.CreateUnifiedGroup("displayName", "description", 
                            "mymodernteamsite", accessToken, groupLogo: groupLogoStream);
            
    // We got group entity as response with available information around the group
    string url = group.SiteUrl;
    string groupId = group.GroupId;

    // Get group based on groupID
    var group2 = UnifiedGroupsUtility.GetUnifiedGroup(groupId, accessToken);
    // Get SharePoint site URL from group id
    var siteUrl = UnifiedGroupsUtility.GetUnifiedGroupSiteUrl(groupId, accessToken);

    // Get all groups from tenant
    List<UnifiedGroupEntity> groups = UnifiedGroupsUtility.ListUnifiedGroups(accessToken);

    // Update description and group logo programatically
    groupLogoStream = new FileStream("C:\\groupassets\\logo-new.png", FileMode.Open, FileAccess.Read);
    UnifiedGroupsUtility.UpdateUnifiedGroup(groupId, accessToken, description: "Updated description", 
                                            groupLogo: groupLogoStream);

    // Delete group programatically
    UnifiedGroupsUtility.DeleteUnifiedGroup(groupId, accessToken);
}
```

### Provisioning a modern team site with PnP PowerShell
<a name="sectionSection0"> </a>
You can also create "modern" sites using [PnP PowerShell](https://github.com/SharePoint/PnP-PowerShell/releases) which will let you easily authenticate towards Microsoft Graph using Azure Active Directory. Following script will create a "modern" team site and will then return the actual SharePoint site URL for further manipulation. When you have access on the URL of the created site, you can use CSOM or SharePoint/PnP PowerShell to automate operations with it.  

```PowerShell
# Connect to Azure AD and get back an OAuth 2.0 Access Token
# This command will prompt sign-in UI to authenticate
Connect-PnPMicrosoftGraph -Scopes "Group.ReadWrite.All","User.Read.All"

# Store the Access Token in a local variable
# This is not really needed for next steps, but is available
$accessToken = Get-PnPAccessToken

# Create a new Office 365 Unified Group, together with the corresponding Modern Site in SPO
$group = New-PnPUnifiedGroup -DisplayName "Awesome Group" -Description "Awesome Group" `
         -MailNickname "awesome-group" -Members "admin@contoso.onmicrosoft.com", "dan@contoso.onmicrosoft.com" `
         -IsPrivate -GroupLogoPath .\logo.jpg

# Connect to the modern site using PnP PowerShell SP cmdlets
# Since we are connecting now to SP side, credentials will be asked
Connect-PnPOnline $group.SiteUrl 

# Now we have access on the SharePoint site for any operations
$context = Get-PnPContext
$web = Get-PnPWeb
$context.Load($web, $web.WebTemplate)
Execute-PnPQuery
$web.WebTemplate + "#" + $web.Configuration
```
> Notice. There is currently no support to provision "modern" team sites using [SharePoint Online Management Shell](https://www.microsoft.com/en-us/download/details.aspx?id=35588).

## Additional Considerations
You cannot provision "modern" team sites using so called app-only approach, since Groups endpoint in Microsoft Graph does not currently support that. This means that you will always need to use specific account when you operated with the modern team sites. This is being looked at, but there's no schedule to provide app-only support for the modern team site creation.

If you provision a sub site under root site of a modern site collection, sub sites are using classic templates. There are currently no modern sub site templates available. You can transform a classic sub site as a modern team site by creating a modern page to the site and updating welcome page of the site to newly created page.  

Modern team sites are not visible in the SharePoint admin UI. You can access the list of modern team sites from the Office 365 Groups admin user interface under Office 365 admin portal. SharePoint Online admin user interface only lists classic SharePoint sites. 


## Additional resources
<a name="bk_addresources"> </a>

-  [Manage site creation in SharePoint Online](https://support.office.com/en-us/article/Manage-site-creation-in-SharePoint-Online-e72844a3-0171-47c9-befb-e98b23e2dcf9?ui=en-US&rs=en-US&ad=US)

