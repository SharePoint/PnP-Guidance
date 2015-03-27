App model recipe - Themes
=========================

Summary
-------

The approach you take to brand SharePoint sites is different in the new app model than it was with Full Trust Code.  In a typical Full Trust Code (FTC) branding scenario, custom master pages, web templates, JavaScript, CSS files, and images are created to implement a custom brand.  These artifacts are typically packaged in a feature which uses declarative code and FTC to deploy the assets and register them with the SharePoint site.

In an app model branding scenario, Themes and composed looks are created to implement a custom brand.  Themes and composed looks are deployed and registered on SharePoint sites via the remote-provisioning pattern.

Why would you custom brand a SharePoint site?
----------------------------------------------------

There are many different reasons why you would apply custom branding to a SharePoint site.  These reasons can include corporate identity, usability, marketing, etc.  

As a rule of a thumb, we would like to provide the following high level guidelines for custom branding SharePoint sites

- Use Office 365 themes, SharePoint site themes, and composed looks to apply branding to SharePoint sites whenever possible
- You can use JavaScript injection to modify or hide elements of a SharePoint site
- You can adjust some CSS settings using the alternate CSS option if the themes do not support your requirements
- Avoid customizing SharePoint sites using custom master pages, since this will cause you additional long term costs and challenges with future updates
	+ In most cases, you can achieve all common branding scenarios with themes, composed looks, and alternate CSS
	+ If you chose to use custom master pages, be prepared to apply changes to the custom master pages when major functional updates are applied to Office 365
- Use remote provisioning to deploy and register themes, composed looks, and all branding artifacts with SharePoint sites
- Do not use declarative code to deploy and register themes, master pages, and all branding artifacts with SharePoint sites  

In summary, customization branding is definitely supported in Office 365 SharePoint Sites. This article will help you consider the short and long term impact of customization from an operational and a maintenance perspective. This is not really specific for SharePoint, rather a rule of thumb for any IT solution built with any platform.

Here’s an example of an Office 365 SharePoint site, which has been customized using the guidelines above. In this case the custom branding has been implemented with an Office 365 theme, deployed, and registered with a SharePoint site via the remote provisioning pattern with the SharePoint CSOM API.

This example comes from the [Theme management using CSOM (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/dev/Samples/Branding.DeployCustomThemeWeb).

![](media/Recipes/Themes/example-custom-theme.png)

Challenges applying brand customization to SharePoint sites
-----------------------------------------------------------

**Office 365 Themes vs. SharePoint Themes**

It is important to understand that Office 365 Themes and SharePoint Themes are different.  It is also important to understand SharePoint themes and composed looks are used to brand SharePoint sites.  This list describes the different items.  

- **Office 365 themes** are used to brand the top navigation bar in an Office 365 tenancy.
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

In general, your rule of thumb is to brand SharePoint sites without using custom master pages whenever possible.

**Deployment**

Custom branding is typically applied when a site is provisioned.  The remote provisioning process fits very well with this approach.  Usually the only time you will use the web browser to manually apply SharePoint branding customization is when you are prototyping or modifying a single SharePoint site that is not planned to grow to include other site collections or sub sites. 

Options to apply brand customization to SharePoint sites
--------------------------------------------------------

There are several options you can use to apply brand customization to SharePoint sites with the new app model.

- Change the composed look for a SharePoint site
- Use the SharePoint color palette tool to create a color palette for a SharePoint theme 
- Create a color scheme for a SharePoint theme manually 
- Create a font scheme for a SharePoint theme manually
- Use JavaScript injection to show and hide components on a SharePoint site
- Create custom master pages
- Create a composed look for a SharePoint site

Change the composed look for a SharePoint Site
----------------------------------------------
Changing a SharePoint site's composed look is the easiest way to apply branding to a SharePoint site.  Composed looks are accessed in the Site Settings page.  SharePoint ships with several composed looks to choose from. 

This option works well when your branding needs are not very specific and you are just looking for a new color scheme and background image for your site.

You can change the composed look for a SharePoint site via the web browser or the remote provisioning pattern.

Use the SharePoint color palette tool to create a color palette for a SharePoint theme
-------------------------------------------------------------------------------------------------------------------------------------------------------
The [SharePoint color palette tool](http://www.microsoft.com/en-gb/download/details.aspx?id=38182) (pictured below) is easy to use and allows you to create the color scheme for a SharePoint theme.  This tool provides a what you see is what you get editing experience.  When you save the color schemes this tool creates it generates a .spcolor file.

![](media/Recipes/Themes/color-palette-tool.png)

This option works well when your branding needs include a new color scheme but do not require layout changes or showing and hiding various Office 365 SharePoint components.

You can use the web browser or the remote provisioning pattern to upload the .spcolor file the tool creates to a SharePoint site.

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

This option works well when your branding needs include a new color scheme but do not require layout changes or showing and hiding various Office 365 SharePoint components.

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

This option works well when your branding needs include a new font scheme but do not require layout changes or showing and hiding various Office 365 SharePoint components.

You can use the web browser or the remote provisioning pattern to upload the .spfont file to a SharePoint site.

Use JavaScript injection to show and hide components on a SharePoint site
-------------------------------------------------------------------------
JavaScript injection may also be used to apply custom branding to SharePoint sites.  JavaScript injection is used when you need to show or hide or modify elements that come with SharePoint.  For example, you could use JavaScript injection to replace the out of the box top navigation control with your own custom client side navigation control.

See this article to learn how to [Customize your SharePoint site UI by using JavaScript](https://msdn.microsoft.com/EN-US/library/dn913116.aspx).  

You can use the remote provisioning pattern to deploy JavaScript injection modifications to a SharePoint site.

Create custom master pages
--------------------------
In scenarios where a custom master page is the only way to implement your custom branding requirements you can create a custom master page.  Keep in mind the points made at the beginning of this article with regard to the long term maintenance costs associated with this approach.

When using a custom master page it is recommended to start with one of the out of the box master pages and modify it to meet your needs.  There are many required content placeholders in SharePoint master pages which must not be removed or they will cause the pages to error.  You will know when you have removed a required content placeholder because the minute you deploy it and assign the master page to your site errors will appear.

Custom master pages may be uploaded manually via the web browser and manually assigned to composed looks.

Custom master pages may be uploaded via the remote provisioning pattern and programatically assigned to composed looks as well.

Create a composed look for a SharePoint Site
----------------------------------------------
A composed look includes the .spcolor and .spfont files described above.  It also include a master page and a background image.  A composed look is not a packaged asset which you deploy to a SharePoint site.  Rather, a composed look is a list item in a special SharePoint list which includes URLs to the master page, .spcolor file, .spfont file, and background image.  When you apply a composed look to a SharePoint site all of these items are set to implement the branding assets the compose look defines.

The following picture illustrates creating a composed look for an Office 365 SharePoint site via the web browser. Notice the portions highlighted in orange.  These highlights indicate the .spcolor and .spfont files described above.  It is important to note that the .spcolor file is referred to as the Theme URL.  This is consistent with the description of a SharePoint theme for and Office 365 SharePoint site.

![](media/Recipes/Themes/new-theme-browser.png)

This option works well when your branding needs are not very specific and you are just looking for a new color scheme, font scheme, and background image for your site.

This option also works well when you need to include a custom master page to implement your branding requirements.

You can upload the assets which make up a composed look via the web browser then create the composed look via the web browser, or you can use the remote provisioning pattern to upload the assets which make up a composed look and create it in the SharePoint list.

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
1.0  | March 27, 2015 | Initial release | Todd Baginski (Canviz LLC)

