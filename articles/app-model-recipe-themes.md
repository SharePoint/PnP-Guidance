App model recipe - Themes
=========================

Summary
-------

The approach you take to brand SharePoint sites is different in the new app model than it was with Full Trust Code.  In a typical Full Trust Code (FTC) branding scenario, custom master pages, web templates, JavaScript, CSS files, and images are created to implement a custom brand.  These artifacts are typically packaged in a feature which uses declarative code and FTC to deploy the assets and register them with the SharePoint site.

In an app model branding scenario, all of the options associated with FTC branding scenarios are available.  Additionally, Office 365 and SharePoint Themes and composed looks may be created to implement a custom brand.  No matter which option you choose, you can deploy and register your branding assets on SharePoint sites via the remote-provisioning pattern.

Why would you custom brand a SharePoint site?
----------------------------------------------------

There are many different reasons why you would apply custom branding to a SharePoint site.  These reasons can include corporate identity, usability, marketing, etc.  

As a rule of a thumb, we would like to provide the following high level guidelines for custom branding SharePoint sites

- Use Office 365 themes, SharePoint site themes, and composed looks to apply branding to SharePoint sites whenever possible
- You can adjust some CSS settings using the Alternate CSS option if the themes do not support your requirements
- You can use JavaScript injection to modify or hide elements of a SharePoint site
- You can customize SharePoint sites using custom master pages, but keep in mind this will cause you additional long term costs and challenges with future updates
	+ In most cases, you can achieve all common branding scenarios with themes, composed looks, and Alternate CSS
	+ If you chose to use custom master pages, be prepared to apply changes to the custom master pages when major functional updates are applied to Office 365
- Use remote provisioning to deploy and register themes, composed looks, and all branding artifacts with SharePoint sites
- Do not use declarative code or sandbox code to deploy and register themes, master pages, and other branding artifacts with SharePoint sites  

In summary, customized branding is definitely supported in Office 365 SharePoint Sites. This article will help you consider the short and long term impact of customization from an operational and a maintenance perspective. This is not really specific for SharePoint, rather a rule of thumb for any IT solution built with any platform.

Here’s an example of an Office 365 SharePoint site, which has been customized using the guidelines above. In this case the custom branding has been implemented with an Office 365 theme, deployed, and registered with a SharePoint site via the remote provisioning pattern with the SharePoint CSOM API.

This example comes from the [Theme management using CSOM (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/dev/Samples/Branding.DeployCustomThemeWeb).

![](media/Recipes/Themes/example-custom-theme.png)

Challenges applying brand customization to SharePoint sites
-----------------------------------------------------------

**Office 365 Themes vs. SharePoint Themes**

It is important to understand that Office 365 Themes and SharePoint Themes are different.  It is also important to understand SharePoint themes and composed looks are used to brand SharePoint sites.  This list describes the different items.  

- **Office 365 themes** are used to brand the top navigation bar in an Office 365 tenancy.  They are only supported in Office 365 SharePoint sites, not on-premises.
- **SharePoint themes** apply colors to your SharePoint sites.
- **Composed looks** apply colors, fonts, master pages, and background images to your SharePoint sites. 

**Office 365 themes** contain the components listed below.  

- custom logo
- url for custom logo
- background image
- base color
- accent color
- nav bar background color
- text and icons color
- app menu icon

See the [Customize the Office 365 theme for your organization](https://support.office.com/en-au/article/Customize-the-Office-365-theme-for-your-organization-8275da91-7a48-4591-94ab-3123a3f79530) article to learn more about Office 365 themes.

**SharePoint themes** include the following components.  

- color palette (.spcolor file)

*Notice a SharePoint theme in an Office 365 SharePoint site does not include a master page, master page preview, or composed look.* This aligns with the guidance mentioned above to not use custom master pages to implement branding on SharePoint sites.

**Composed looks used for on-premises SharePoint 2013 sites** include the following components.  

- color palette (.spcolor file) - Also referred to as a SharePoint theme
- font scheme (.spfont file)
- background image
- master page
- master page preview

See the [Themes overview for SharePoint 2013](https://msdn.microsoft.com/en-us/library/office/jj927174.aspx) article to learn more about these components.

**Composed looks used for Office 365 SharePoint 2013 sites** include the following components.  

- color palette (.spcolor file) - Also referred to as a SharePoint theme
- font scheme (.spfont file)
- background image
- master page

**Team Sites vs. Publishing Sites**

When applying custom branding to SharePoint sites you will encounter the need to brand both Team sites and Publishing sites. Generally speaking, Intranets built on SharePoint in both on-premises and Office 365 scenarios use a combination of Team sites and Publishing sites.  

Custom branding requirements often times require specific layout changes which themes and JavaScript injection techniques cannot accomplish.  A responsive web design is a good example of when a custom master page is required.  

In such a scenario, Team sites usually do not require the amount of custom branding that Publishing sites do and the out of the box SharePoint Contemporary View for mobile devices is usually sufficient to support mobile devices for Team sites.  Since this is the case it is best to only use custom Master Pages for Publishing sites and to use custom SharePoint themes (.spcolor files), font schemes (.spfont files), and background images defined as composed looks to brand Team sites.

**Deployment**

Custom branding is typically applied when a site is provisioned.  The remote provisioning process fits very well with this approach.  Usually the only time you will use the web browser to manually apply SharePoint branding customization is when you are prototyping or modifying a single SharePoint site that is not planned to grow to include other site collections or sub sites. 

Options to apply brand customization to SharePoint sites
--------------------------------------------------------

There are several options you can use to apply brand customization to SharePoint sites with the new app model.

- Use an Office 365 theme to brand a SharePoint site
- Change the composed look for a SharePoint site
- Use the SharePoint color palette tool to create a color palette for a SharePoint theme 
- Use Alternate CSS to brand a SharePoint site
- Create a color scheme for a SharePoint theme manually 
- Create a font scheme for a SharePoint theme manually
- Use JavaScript injection to show and hide components on a SharePoint site
- Create custom master pages and page layouts for a SharePoint site
- Create a composed look for a SharePoint site

Use an Office 365 theme to brand a SharePoint site
--------------------------------------------------

Changing an O365 tenancy's Office theme is the easiest way to apply branding to a SharePoint site.

- Office 365 Themes can be used to centrally control branding across all Office 365 services.
	+ Currently, the amount of settings associated with an Office 365 theme is limited
- Office 365 themes may be overridden at the SharePoint site level
- Office 365 themes only exist in Office 365 tenants, not in on-premises SharePoint
- Office 365 themes provide a fair amount of flexibility to brand a SharePoint site
- Office 365 themes are very easy and inexpensive to implement and maintain in the short and long term

**When is it a good fit?**

This option works well when your branding needs are not very specific and you are just looking for a new color scheme for the Office bar portion of your SharePoint site, a logo, and a background image.  ***It is important to note that the only way to change the App Menu icon is via the Office 365 theme.***

**Recommended deployment approaches**

You can change the Office 365 theme for an Office 365 tenancy via the web browser or the remote provisioning pattern.

Change the composed look for a SharePoint site
----------------------------------------------
Changing a SharePoint site's composed look is another easy way to apply branding to a SharePoint site.  

- Composed looks are accessed in the Site Settings page.  
- SharePoint ships with several composed looks to choose from.
- Composed looks exist in both Office 365 tenants and in on-premises SharePoint
- Composed looks provide a fair amount of flexibility to brand a SharePoint site.
	+ Remember, composed looks are collections of color and font schemes, a background image, and a master page.
- Composed looks are very easy and inexpensive to implement in the short and long term
- Composed looks can include out of the box master pages, or custom master pages
- You can use composed looks at a per site level
 
**When is it a good fit?**

This option works well when your branding needs are not very specific and you are just looking for a new color scheme, background image, and a master page for your site.

**Recommended deployment approaches**

You can change the composed look for a SharePoint site via the web browser or the remote provisioning pattern.

Use the SharePoint color palette tool to create a color palette for a SharePoint theme
--------------------------------------------------------------------------------------
The [SharePoint color palette tool](http://www.microsoft.com/en-gb/download/details.aspx?id=38182) (pictured below) is easy to use and allows you to create the color scheme for a SharePoint theme.  This tool provides a what you see is what you get editing experience.  When you save the color schemes this tool creates it generates a .spcolor file.

![](media/Recipes/Themes/color-palette-tool.png)

- Creating custom color schemes for SharePoint sites is very easy and inexpensive to implement and maintain in the short and long term
	+ Keep in mind, a custom color scheme is just one piece of a composed look
- Custom color schemes provide a fair amount of flexibility to brand a SharePoint site
- You can apply color schemes via composed looks at a per site level

**When is it a good fit?**

This option works well when your branding needs include a new color scheme but do not require layout changes or showing and hiding various Office 365 SharePoint components.

**Recommended deployment approaches**

You can use the web browser or the remote provisioning pattern to upload the .spcolor file the tool creates to a SharePoint site, create a composed look which includes it, and apply it to a SharePoint site.

Use Alternate CSS to brand a SharePoint site
--------------------------------------------
You can also create a custom Cascading Style Sheet (CSS) file and set it as the Alternate CSS file for a SharePoint site.  

- Alternate CSS may be used to override whatever out of the box CSS settings that come with SharePoint
- You can use the Alternate CSS approach to control to color, fonts and even layout settings 
- Alternate CSS requires a medium amount of investment to implement and maintain in the short and long term
- Alternate CSS provides a good amount of flexibility to brand a SharePoint site
- You can use Alternate CSS at a per site level

**When is it a good fit?**

This option works well when your branding needs include a new color scheme, fonts, and require minimal layout changes but do not include showing and hiding various Office 365 SharePoint components.

**Recommended deployment approach**

You can use the web browser or the remote provisioning pattern to upload the a CSS file to a SharePoint site and apply it to a SharePoint site.

Create a color scheme for a SharePoint theme manually
------------------------------------------------------
You can also create a .spcolor file manually with a text editor such as Notepad or Visual Studio.  An example snippet from a .spcolor file is shown below.

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:colorPalette isInverted="false" previewSlot1="BackgroundOverlay" previewSlot2="BodyText" previewSlot3="AccentText" xmlns:s="http://schemas.microsoft.com/sharepoint/">
<s:color name="BodyText" value="444444" />
<s:color name="SubtleBodyText" value="777777" />
<s:color name="StrongBodyText" value="262626" />
```

- Creating custom color schemes for SharePoint sites is very easy and inexpensive to implement and maintain in the short and long term
	+ Keep in mind, a custom color scheme is just one piece of a composed look
- Custom color schemes provide a fair amount of flexibility to brand a SharePoint site
- You can apply color schemes via composed looks at a per site level
 
**When is it a good fit?**

This option works well when your branding needs include a new color scheme but do not require layout changes or showing and hiding various Office 365 SharePoint components.

**Recommended deployment approaches**

You can use the web browser or the remote provisioning pattern to upload the .spcolor file the tool creates to a SharePoint site.

Create a font scheme for a SharePoint theme manually
----------------------------------------------------
You can also define the fonts your SharePoint site uses by making a font scheme for your SharePoint site.  The .spfont file must be manually created with a text editor such as Notepad or Visual Studio.  An example snippet from a .spfont file is shown below.

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:fontScheme name="Bodoni" previewSlot1="title" previewSlot2="body" xmlns:s="http://schemas.microsoft.com/sharepoint/">
    <s:fontSlots>
        <s:fontSlot name="title">
            <s:latin typeface="Bodoni Book" eotsrc="/_layouts/15/fonts/BodoniBook.eot" woffsrc="/_layouts/15/fonts/BodoniBook.woff" ttfsrc="/_layouts/15/fonts/BodoniBook.ttf" svgsrc="/_layouts/15/fonts/BodoniBook.svg" largeimgsrc="/_layouts/15/fonts/BodoniBookLarge.png" smallimgsrc="/_layouts/15/fonts/BodoniBookSmall.png" />
            <s:ea typeface="" />
            <s:cs typeface="Segoe UI Light" />
            <s:font script="Arab" typeface="Segoe UI Light" />
```


- Creating custom font schemes for SharePoint sites is very easy and inexpensive to implement and maintain in the short and long term.  
	+ Keep in mind, a custom font scheme is just one piece of a composed look.
- Custom font schemes provide a fair amount of flexibility to brand a SharePoint site
- You can apply font schemes via composed looks at a per site level

**When is it a good fit?**

This option works well when your branding needs include a new font scheme but do not require layout changes or showing and hiding various Office 365 SharePoint components.

**Recommended deployment approaches**

You can use the web browser or the remote provisioning pattern to upload the .spfont file to a SharePoint site.

Use JavaScript injection to show and hide components on a SharePoint site
-------------------------------------------------------------------------
JavaScript injection may also be used to apply custom branding to SharePoint sites.  JavaScript injection registers JavaScript to execute for all pages on a SharePoint site.  Under the hood, JavaScript injection relies on custom actions assigned to script block definitions.  These custom actions are added to the SharePoint site and cause the JavaScript in the script blocks to execute.  In summary, this approach allows you to execute JavaScript code.  In a branding scenario, the JavaScript code typically uses JQuery to maniuplate the Document Object Model (DOM).

See this article to learn how to [Customize your SharePoint site UI by using JavaScript](https://msdn.microsoft.com/EN-US/library/dn913116.aspx).  

- Using JavaScript injection for SharePoint sites requires a medium amount of time to implement and maintain in the short and long term
- Using JavaScript injection for SharePoint sites provides a good amount of flexibility to brand a SharePoint site
- You can apply JavaScript injection at a per site level
- When Minimal Download /Strategy (MDS) is enabled for a SharePoint site you must take extra care to ensure any JavaScript injection you use will perform correctly.  The article referenced above describes this in depth.

**When is it a good fit?**

This option works well when you need to show or hide or modify elements that come with SharePoint.  For example, you could use JavaScript injection to replace the out of the box top navigation control with your own custom client side navigation control.

**Recommended deployment approach**

You can use the remote provisioning pattern to deploy JavaScript injection modifications to a SharePoint site.

Create custom master pages and page layouts for a SharePoint site
-----------------------------------------------------------------
In scenarios where a custom master page is the only way to implement your custom branding requirements you can create a custom master page and page layouts.  This is the approach used to brand Publishing sites.  Keep in mind the points made at the beginning of this article with regard to the long term maintenance costs associated with this approach.

- Using custom master pages for SharePoint sites provides the ultimate level of customization (unlimited)
- Using custom master pages for SharePoint sites requires the largest amount of time to implement and maintain in the short and long term
- Any changes to out of the box master pages that come with service updates will not be reflected in custom master pages
- You can apply custom master pages at a per site level
- When using a custom master page it is recommended to start with one of the out of the box master pages and modify it to meet your needs.
	+ Try to minimize he amount of customization you make with custom master pages, this will make it easier to update them when O365 service changes to out of the box master pages must be replicated to custom master pages  
- There are many required content placeholders in SharePoint master pages which must not be removed or they will cause the pages to error.  You will know when you have removed a required content placeholder because the minute you deploy it and assign the master page to your site errors will appear.

**When is it a good fit?**
This option works well when your branding needs are very specific or you are using Publishing sites. Responsive Web Design requirements are a good example of specific branding requirements which are best implemented via a custom master page.

**Recommended deployment approaches**

Custom master pages may be uploaded manually via the web browser and manually assigned to composed looks.

Custom master pages may be uploaded and assigned to a SharePoint site via the remote provisioning pattern as well.

Create a composed look for a SharePoint Site
----------------------------------------------
A composed look includes the .spcolor and .spfont files described above.  It also include a master page and a background image.  A composed look is not a packaged asset which you deploy to a SharePoint site.  Rather, a composed look is a list item in a special SharePoint list which includes URLs to the master page, .spcolor file, .spfont file, and background image.  When you apply a composed look to a SharePoint site all of these items are set to implement the branding assets the compose look defines.

The following picture illustrates creating a composed look for an Office 365 SharePoint site via the web browser. Notice the portions highlighted in orange.  These highlights indicate the .spcolor and .spfont files described above.  It is important to note that the .spcolor file is referred to as the Theme URL.  This is consistent with the description of a SharePoint theme for an Office 365 SharePoint site.

![](media/Recipes/Themes/new-theme-browser.png)

- Using composed looks for SharePoint sites provides a good level of customization
- Using composed looks for SharePoint sites requires a small amount of time to implement and maintain in the short and long term
- You can apply composed looks at a per site level

**When is it a good fit?**

This option works well when your branding needs are not very specific and you are just looking for a new color scheme, font scheme, and background image for your site.

This option also works well when you need to include a custom master page to implement your branding requirements.

**Recommended deployment approaches**

You can upload the assets which make up a composed look via the web browser then create the composed look via the web browser, or you can use the remote provisioning pattern to upload the assets which make up a composed look and create it in the SharePoint list.

Summary
-------
The following chart summarizes all your options to brand a SharePoint site at a high level.

![](media/Recipes/Themes/option-comparison-chart.png)

Related links
=============
- [SharePoint color palette tool](http://www.microsoft.com/en-gb/download/details.aspx?id=38182)
- [Customize your SharePoint site UI by using JavaScript](https://msdn.microsoft.com/EN-US/library/dn913116.aspx)
- Guidance articles at [http://aka.ms/OfficeDevPnPGuidance](http://aka.ms/OfficeDevPnPGuidance "Guidance Articles")
- References in MSDN at [http://aka.ms/OfficeDevPnPMSDN](http://aka.ms/OfficeDevPnPMSDN "References in MSDN")
- Videos at [http://aka.ms/OfficeDevPnPVideos](http://aka.ms/OfficeDevPnPVideos "Videos")

Related PnP samples
===================

- [Theme management using CSOM (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/dev/Samples/Branding.DeployCustomThemeWeb)
- [Set theme to site (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/dev/Samples/Branding.SetThemeToSite)
- [Setting a SharePoint Theme in an App for SharePoint (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/dev/Scenarios/Branding.Themes)
- Samples and content at https://github.com/OfficeDev/PnP

Applies to
==========
- Office 365 Multi Tenant (MT)
- Office 365 Dedicated (D) *partly*
- SharePoint 2013 on-premises – *partly*

**Need to know all the possible choices we can have here and the exact names for them.**

*Patterns for Dedicated and on-premises are identical with app model techniques, but there are differences on the possible technologies which can be used.*

Author
------
Todd Baginski (Canviz LLC) - [@toddbaginski](https://twitter.com/toddbaginski)

Version history
---------------
Version  | Date | Comments
---------| -----| --------
0.1  | March 27, 2015 | Initial draft | Todd Baginski (Canviz LLC)
0.2  | March 30, 2015 | Revisions based on feedback from Vesa | Todd Baginski (Canviz LLC)

