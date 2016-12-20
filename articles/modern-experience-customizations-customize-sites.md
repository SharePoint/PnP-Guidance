# Customizing modern team sites
During autumn 2016 the SharePoint Online team released "modern" collaboration sites. These modern team sites are integrated with Office 365 groups and they have numerous enhancements from the end user experience. "Modern" team sites are natively responsive and they are much faster to create and use from end user perspective. 

This article concentrates on the available extensibility options in "modern" team sites. Here are key links around the key capabilities. 

- New capabilities in SharePoint Online team sites including integration with Office 365 Groups: https://blogs.office.com/2016/08/31/new-capabilities-in-sharepoint-online-team-sites-including-integration-with-office-365-groups
- Create connected SharePoint Online team sites in seconds: https://blogs.office.com/2016/11/08/create-connected-sharepoint-online-team-sites-in-seconds
- [Turn scripting capabilities on or off](https://support.office.com/en-us/article/Turn-scripting-capabilities-on-or-off-1f2c515f-5d7e-448a-9fd7-835da935584f) - Notice that you cannot enable scripting capabilities in the modern team sites, but this article defines the features, which are affected when scripting is disabled

_**Applies to:** SharePoint Online_

## Supported customizations in modern team sites
<a name="supportedcustomizations"> </a>
Below list gives a quick overview of the supported capabilities for "modern" team sites.

- Apply a custom theme 
- Apply out of the box theme
- Custom Site columns (fields) and content types
- Lists and libraries
- Site configurations, like regional settings, languages and auditing settings
- Apply oob themes

> Notice. You can apply a custom theme, but you cannot introduce a custom theme to theme gallery as an option for the end users.

### What's not supported with "modern" team sites?
There are numerous areas in the modern team sites where the typical customizations are not yet available. There will be further support for some of these specific topics when they are ready to be released. 

- Custom master pages - More extensive branding will be supported later using alternative options
- Custom page layouts - We are looking to have support for multiple canvases in in future
- Welcome page modifications - There are no APIs to modify the welcome page current, this will be introduced later
- User custom actions / Custom JavaScript - There will be more controlled way to embed JavaScript on the pages through SharePoint Framework (not only client-side web parts)
- "Modern" sub sites - Sub sites created in "modern" team sites are using classic experience
- Control available sub site template options
- Classic publising features (WCM)
- Accessing or updating site property bag entries

Since "modern" team sites have also the scripting capabilities disabled, there are numerous areas, which cannot be customized using the classic models. Here are some key areas, which should be taken into account while you are designing your deployment.

- Sandbox solutions are not supported
- Custom JavaScript cannot be enabled in the sites using classic scenarios
- You cannot access sites using SharePoint Designer
- Some web parts are not available for end users

> You can find full list of impacted capabilities from the [Microsoft Support article](https://support.office.com/en-us/article/Turn-scripting-capabilities-on-or-off-1f2c515f-5d7e-448a-9fd7-835da935584f) under the "Features affected when scripting is disabled" chapter.


### Using PnP Provisioning Engine with "modern" team sites
<a name="pnpprovisioningengine"> </a>
You can use the PnP Provisioning Engine with modern team sites. PnP Provisioning Engine will detect if site is a "modern" team site and will automatically adjust it's behaviour based on the supported capabilities. Process is exactly the same if you use PnP Provisioning Engine with "classic" sites where the scripting capabilities are disabled.

Following elements are ignored when a remote template is applied to a "modern" team site or a site which has "no scripting" enabled.
- Site collection AuditLogTrimmingRetention configuration in the auditing settings
- Apply a custom theme from the template - Current implementation has dependency on storing custom theme to catalog, which is not supported
- Form settings for content types
- Adding custom user actions to site or list level 
- Adding files with file types of ".asmx", ".ascx", ".aspx", ".htc", ".jar", ".master", ".swf", ".xap", ".xsf"
- Adding files to libraries with following url  "_catalogs/theme", "style library", "_catalogs/lt", "_catalogs/wp" 
- Adding web parts to site pages
- Storing provisioning template information to property bag of the provisioned site
- Adding or updating property bag entries to site property bag
- Classic publishing settings and assets
- Site No Crawl settings
- Site master page settings

## Applying custom theme to modern team site
<a name="sectionSection0"> </a>
"Modern" team sites do support custom themes even though you cannot upload new gallery entry for end users. This can be achieved by uploading needed assets to the site and executing ApplyTheme method for the site. Following PowerShell script shows how to perform this for "modern" team site.

```PowerShell

# Connect to a previously created Modern Site
$cred = Get-Credential
Connect-PnPOnline https://[tenant].sharepoint.com/sites/siteurl -Credentials $cred

# Apply a custom theme to a Modern Site

# First, upload theme assets
Add-PnPFile -Path .\sppnp.spcolor -Folder SiteAssets
Add-PnPFile -Path .\sppnp-bg.png -Folder SiteAssets

# Second, apply theme assets to site
$palette = $web.ServerRelativeUrl + "/SiteAssets/sppnp.spcolor"
$background = $web.ServerRelativeUrl + "/SiteAssets/sppnp-bg.png"

# We use oob CSOM operation for this
$web.ApplyTheme($palette, [NullString]::Value, $background, $true)
$web.Update()
# Set timeout as high as possible and execute
$web.Context.RequestTimeout = [System.Threading.Timeout]::Infinite
$web.Context.ExecuteQuery()

```

> You can use [SharePoint Color Palette Tool](https://www.microsoft.com/en-us/download/details.aspx?id=38182) to create a custom theme file (.spcolor) with the custom color definition.

## How to determine if a site is a modern team site?
<a name="sectionSection0"> </a>
You can detect that a site is a modern team site by checking the 'Web.WebTemplate' value of the site. Modern team site is using "GROUP" template. Since supported capabilities are the same for "classic" team site when the scripting is disabled, you should be checking these both settings in general for your code to determine the right behaviour or supported capabilities.

Since there's no direct property to check if the scripting is enabled or not, you can use permissions to determine the current status. When scripting is enabled, there's no AddAndCustomizePages permission in the base permissions of the site.

```C#
        /// <summary>
        /// Can be used to check if site has no scripting enabled.
        /// </summary>
        /// <param name="web">site object to inspect</param>
        /// <returns>True if no scripting is enabled, False if it's not</returns>
        public static bool IsNoScriptSite(Web web)
        {
            // Array if there will be more of these specific tempates 
            string[] NoScriptSiteTemplates = new string[] { "GROUP" };

            // Ensure that we have the needed properties - Notice that these are 
            // PnP CSOM extension capabilities
            web.EnsureProperties(w => w.WebTemplate, w => w.EffectiveBasePermissions);

            // If we know that template is no script site
            if (NoScriptSiteTemplates.Contains(web.WebTemplate))
            {
                return true;
            }

            // Definition of no-script is not having the AddAndCustomizePages permission
            if (!web.EffectiveBasePermissions.Has(PermissionKind.AddAndCustomizePages))
            {
                return true;
            }

            // It's a "classic" site without no script enabled settings
            return false;
        }

'''

## Considerations
Considerations and things to be aware
- We will add additional customization capabilities to modern team sites gradually


## Additional resources
<a name="bk_addresources"> </a>

-  [PnP Remote Provisioning](https://msdn.microsoft.com/en-us/pnp_articles/pnp-remote-provisioning)

