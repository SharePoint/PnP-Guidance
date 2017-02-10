# Customizing "modern" site pages
During the autumn of 2016 the "modern" page experience was released by the SharePoint team. Modern team site pages are fast, easy to author, and support rich multimedia content. Additionally, pages look great on any device, in a browser or from within the SharePoint mobile app. SharePoint pages are built with web parts, which you can customize according to your needs. You can add documents, videos, images, site activities, Yammer feeds, and more. Just click the + sign and pick a web part from the toolbox to add content to your page. The new “highlighted content” web part lets you set criteria so that specific content will automatically and dynamically populate in that area of the page. And using the SharePoint Framework, developers can build custom web parts that will show up right in the toolbox.

![](https://blogs.office.com/wp-content/uploads/2016/08/New-capabilities-in-SharePoint-Online-team-sites-including-integration-with-Office-365-Groups-1.gif)

This article focuses on the extensibility options within the "modern" page experience. If you, however, want to learn more about the functionalities offered by the "modern" experiences, then the following link will help:
 - New capabilities in SharePoint Online team sites: https://blogs.office.com/2016/08/31/new-capabilities-in-sharepoint-online-team-sites-including-integration-with-office-365-groups

In the remainder of this article we'll use "modern" for the new user experience and "classic" for the legacy user experience. 

>**Important:** 
We're not deprecating the "classic" experience - both "classic" and "modern" will coexist.

_**Applies to:** SharePoint Online_


## Supported customizations for "modern" pages
The number of customizations available for "modern" pages is limited and in this article we'll provide details and examples of the supported options. The SharePoint team is working to support more options in the future. The list below gives a quick overview of the supported capabilities for "modern" team sites:
 - Custom branding

There are numerous customizations which currently are not supported for "modern" pages:
 - Alternative layouts -  We are looking to have support for multiple canvases in the future
 - Custom page templates (layout templates) - We are looking to have support for multiple canvases in the future
 - Adding "classic" web parts on "modern" pages
 - Custom CSS via AlternateCSSUrl web property
 - Custom JavaScript embedded via User Custom Actions - There will a be more controlled way to embed JavaScript on the pages through SharePoint Framework (not only client-side web parts)
 - Custom master pages - More extensive branding will be supported later using alternative options
 - Programmatically adding "modern" pages - More options will become available in the future
 - Minimal Download Strategy (MDS)
 - SharePoint Server Publishing

## Custom branding
<a name="themingimpact"> </a>
If your site happens to use a custom theme, then this custom theme will be respected in the "modern" page experience as shown in the sample below:

![Modern page with custom branding coming from theme settings](media/modern-experiences/modern-page-with-custom-theme.png)

## How to configure the end user experience
<a name="configuremodernpages"> </a>
You have multiple options to control whether the "modern" or "classic" page experience will be used. 

### Tenant level configuration
If you want to completely disable the "modern" experience, then it's best to use the tenant setting for this. Navigate to your tenant admin center (e.g. contoso-admin.sharepoint.com), go to settings, and select the "classic" experience:

![Site Pages section in the SharePoint tenant scoped settings in admin UI](media/modern-experiences/site-pages-setting-admin-ui.png)

>**Notes:**
> - The tenant level setting can be a little confusing: "Preventing users from creating Site Pages" will actually bring back the "classic" experience.
> - The current configuration is cached, logging off the session will immediately show the effect of this change.

### Site level configuration
You can prevent a site collection or web from using the "modern" page experience by disabling the site collection scoped feature with ID **B6917CB1-93A0-4B97-A84D-7CF49975D4EC**. To re-enable the "modern" page experience at the site level you'll need to activate the feature again.

You can use the [PnP provisioning XML](https://msdn.microsoft.com/en-us/pnp_articles/pnp-provisioning-engine-and-the-core-library) below to **disable** this feature on your site collection:

```XML
<pnp:ProvisioningTemplate ID="disablemodernpages" Version="1" xmlns:pnp="http://schemas.dev.office.com/PnP/2015/12/ProvisioningSchema">
  <pnp:Features>
    <pnp:SiteFeatures>
      <pnp:Feature ID="B6917CB1-93A0-4B97-A84D-7CF49975D4EC" Deactivate="true" Description="Disable modern list experience"/>
    </pnp:SiteFeatures>
  </pnp:Features>
</pnp:ProvisioningTemplate>
```

You can use the [PnP provisioning XML](https://msdn.microsoft.com/en-us/pnp_articles/pnp-provisioning-engine-and-the-core-library) below to **enable** this feature on your site collection:

```XML
<pnp:ProvisioningTemplate ID="enablemodernpages" Version="1" xmlns:pnp="http://schemas.dev.office.com/PnP/2015/12/ProvisioningSchema">
  <pnp:Features>
    <pnp:SiteFeatures>
      <pnp:Feature ID="B6917CB1-93A0-4B97-A84D-7CF49975D4EC" Description="Disable modern list experience"/>
    </pnp:SiteFeatures>
  </pnp:Features>
</pnp:ProvisioningTemplate>
```

Use the following PnP PowerShell to apply this template:

```PowerShell

# Connect to a previously created Modern Site
$cred = Get-Credential
Connect-PnPOnline -Url https://[tenant].sharepoint.com/sites/siteurl -Credentials $cred

# Apply the PnP provisioning template
Apply-PnPProvisioningTemplate -Path c:\experiencecontrol.xml -Handlers Features

```

## Additional Considerations
<a name="sectionSection22"> </a>

We'll gradually introduce more customization options for the "modern" pages experience. These options will be aligned with the release of additional SharePoint framework capabilities. Currently there is no exact schedule available, but we'll be updating the "modern" experience articles whenever new capabilities are released.

## Additional resources
<a name="bk_addresources"> </a>

 - [Allow or prevent creation of site pages by end users](https://support.office.com/en-us/article/Allow-or-prevent-creation-of-site-pages-by-end-users-c41d9cc8-c5c0-46b4-8b87-ea66abc6e63b?ui=en-US&rs=en-US&ad=US)
