# Customizing modern team sites
Introduction to topic and what's the objective of the article.

_**Applies to:** SharePoint Online_

## Supported customizations in modern team sites
<a name="supportedcustomizations"> </a>

Supported customizations or configurations what can be done in the modern team sites

- Apply a custom theme 
- Apply out of the box theme
- Custom Site columns (fields) and content types
- Lists and libraries
- Site configurations, like regional settings, languages and auditing settings
- Apply oob themes

> Notice. You can apply a custom theme, but you cannot introduce a custom theme to theme gallery as an option for the end users.


### What's not supported with modern team sites?
There are numerous areas in the modern team sites where the typical customizations are not yet available. There will be further support for some of these specific topics when they are ready to be released.

- Custom master pages - More extensive branding will be supported later using alternative options
- Custom page layouts - We are looking to have support for multiple canvases in in future
- Welcome page modifications - There are no APIs to modify the welcome page current, this will be introduced later
- User custom actions / Custom JavaScript - There will be more controlled way to embed JavaScript on the pages through SharePoint Framework (not only client-side web parts)
- Modern sub sites - Sub sites created in modern team sites are using classic experience
- Control available sub site template options
- Classic publising features (WCM)
- Accessing or updating site property bag entries

Since modern team sites have also the scripting capabilities disabled, there are numerous areas, which cannot be customized using the classic models. Here are some key areas, which should be taken into account while you are designing your deployment.

- Sandbox solutions are not supported
- Custom JavaScript cannot be enabled in the sites using classic scenarios
- You cannot access sites using SharePoint Designer
- Some web parts are not available for end users

You can find full list of impacted capabilities from the [Microsoft Support article](https://support.office.com/en-us/article/Turn-scripting-capabilities-on-or-off-1f2c515f-5d7e-448a-9fd7-835da935584f) under the "Features affected when scripting is disabled" chapter.


### Using PnP Provisioning Engine with modern team sites
<a name="pnpprovisioningengine"> </a>
Explain what's supported from remote template perspective.

- Reference existing articles on this

## Applying custom theme to modern team site
<a name="sectionSection0"> </a>
Introduction

## How to determine if a site is a modern team site?
<a name="sectionSection0"> </a>
Template + no script story

## Considerations
Considerations and things to be aware
- We will add additional customization capabilities to modern team sites gradually


## Additional resources
<a name="bk_addresources"> </a>

-  [PnP Remote Provisioning](https://msdn.microsoft.com/en-us/pnp_articles/pnp-remote-provisioning)

