App model recipe - Site Columns and Content Types
=================================================

Summary
-------

The approach you take to create site columns and content types in SharePoint sites is different in the new app model than it was with Full Trust Code.  In a typical Full Trust Code (FTC) / Farm Solution scenario, site columns and content types are created with declarative code.  In the declarative code approach the site columns and content types are defined in XML and SharePoint's feature framework elements are used to package and deploy them.

In an app model scenario, site columns and content types are created with the SharePoint Client Side Object Model (CSOM) or SharePoint REST APIs.

High Level Guidelines
---------------------

As a rule of a thumb, we would like to provide the following high level guidelines for creating site columns and content types.

- The SharePoint CSOM or REST APIs should be used to create site columns and content types.
- Feature framework elements should not be used in the creation of site columns and content types.
	+ The only exception to this guideline is when you are using declarative XML-based provisioning to an app web in a SharePoint-hosted app.  This is due to the fact that the CSOM is not available in a SharePoint-hosted app.
- You can automate the creation of site columns and content types as part of the site provisioning process.  See the [site provisioning recipe](/articles/app-model-recipe-site-provisioning.md) for more details.

Challenges creating site columns and content types in SharePoint sites
----------------------------------------------------------------------

**Creating in a web browser vs. Creating with code** 

It is important to understand that creating site columns and content types via the web browser or via code are different.  This list describes the different options.

- **Creating via a web browser**
	+ In this option, users access a SharePoint site via a web browser and use the Administrative Pages to create site columns and content types.
	+ Usually the only time you will use the web browser to manually create site columns and content types is when you are prototyping or modifying a single SharePoint site that is not planned to grow to include other site collections or sub sites.
- **Creating with code**
	+ In this option, SharePoint CSOM/REST code is executed to create site columns and content types.
	+ There are a few options you can use to execute the SharePoint CSOM/REST code, they are described later in this article.

When **Creating via a web browser** consider the following points.

- Creating site columns and content types via the web browser is typically a complicated and time consuming process.
	+ These factors make it **prone to error**.
- You do not control the GUIDs for site columns or content types when created via a web browser.
	+ This makes it **difficult** to deploy the site columns and content types to different environments and reference them in line of business applications consistently.

When **Creating with code** consider the following points.

- Creating site columns and content types with code typically involves using custom utility libraries to execute SharePoint CSOM/REST code.
	+ These libraries are available in many projects in the OfficeDev PnP GitHub Repository.  They are referenced throughout the article and at the end.
	+ These factors make it **prone to success**.
- You can control the GUIDs for site columns or content types when created via the SharePoint CSOM/REST.
	+ This makes it **easy** deploy the site columns and content types to different environments and reference them in line of business applications consistently.

**Must happen quickly!**

The creation of site columns and content types typically happens when a SharePoint site is provisioned.  End users won't accept having to wait several hours for their new SharePoint sites to be provisioned.

**Must be consistently perfect!**

Site columns and content types are the foundation which define your information architecture at the lowest level, *they must be perfect*!

Incorrect site column and content type provisioning can affect an entire line of business application in the SharePoint site where they are provisioned as well as other parts of SharePoint and other line of business applications which access SharePoint services.

For example:  If you have SharePoint sites used to manage projects in your company you will most likely create a common list schema for all of them.  This will require creating site columns and content types.  When you search for information in these sites via the SharePoint search page you filter the results by content type or tag (site column). If your site columns and content types are not perfectly consistent across all the project sites you will not receive accurate search results.

This example may also be applied to Content By Search Web Parts, SharePoint apps, mobile apps, and any other systems which access the information in the SharePoint sites.

Options to create site columns and content types in SharePoint sites
--------------------------------------------------------------------

There are several ways you can call the CSOM/REST code to create site columns and content types.  These patterns all fall into the **Creating with code** approach described above.  Each one of these patterns is described in detail in the [site provisioning recipe](/articles/app-model-recipe-site-provisioning.md).

- Override the create site link
- Override the create sub site link
- Use a Provider-hosted app
- Use Windows/Java/iOS applications or PowerShell scripts

Regardless of the option you choose to implement, you will ultimately use CSOM/REST to create site columns and content types.

There are many different articles and samples you can use to learn how to make site columns and content types with the CSOM.  Here you will find these examples (classified by the pattern that is used to invoke the CSOM code) to create site columns and content types.

Use a Provider-hosted app
-------------------------
This option works well when you need to provide your end users with a self-service ability to create SharePoint site collections and sub sites based on custom templates.

- [Core.ContentTypesAndFields (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/dev/Scenarios/Core.ContentTypesAndFields)
	+ Demonstrates how to create a new content type in the host web, create a taxonomy field in the host web and wire it up to the taxonomy, create a list and associate it with a content type, create content types and fields in particular languages.

Use Windows/Java/iOS applications or PowerShell scripts
-------------------------------------------------------

This option works well in Dev-Ops scenarios. It allows you to create custom applications or scripts that are specifically built to work with your Dev-Ops processes. This option provides the ultimate level of automation because the apps and scripts can be built to run without any user interaction.  

- [Core.CreateContentTypes (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/dev/Samples/Core.CreateContentTypes)
	+ This sample shows how you can create site columns, content types and add then add the site columns to the content type. It also explains the new localization features that have been introduced for Office 365 CSOM APIs.
- [Core.CreateDocumentContentType (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/dev/Samples/Core.CreateDocumentContentType)
	+ This sample shows how you can create document content types and add then associate a document template to the content type.

More Examples
-------------

- [Branding.DisplayTemplates (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/master/Samples/Branding.DisplayTemplates)
	+ The Display Templates sample demonstrates how to use Display Templates to render a hero image and content rotator in a Content By Search Web Part. Additionally, the Display Templates target mobile devices using Responsive Web Design (RWD) and Device Channels.
	+ The [code behind for the default.aspx web page](https://github.com/OfficeDev/PnP/blob/master/Samples/Branding.DisplayTemplates/Branding.DisplayTemplatesWeb/Pages/Default.aspx.cs) is an excellent easy to follow example that demonstrates how to create a list, create a content type for the list, bind site columns to the content type, bind the content type to the list, upload control and item template JS files to the master page gallery, upload master pages, create pages and add content and web parts to the pages, and initialize list data.  
- [Core.DataStorageModels (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/master/Samples/Core.DataStorageModels)
	+ This Provider-hosted sample application for SharePoint demonstrates the differences, advantages, and disadvantages between different data storage patterns associated with the App Model and how they are built. It also illustrates limitations associated with certain data storage components that should be considered when deciding which data storage components to use when building with the App Model.  
	+ The [Util class](https://github.com/OfficeDev/PnP/blob/master/Samples/Core.DataStorageModels/Core.DataStorageModelsWeb/Util/Util.cs) includes reusable methods which may be used to create site columns and content types.  
	+ The [SharePointService class](https://github.com/OfficeDev/PnP/blob/master/Samples/Core.DataStorageModels/Core.DataStorageModelsWeb/Services/SharePointService.cs)  includes methods which demonstrate how to create lists, content types, and site columns and many other related operations.


Related links
=============
- [App Model Recipe - Site Provisioning (O365 PnP Recipe)](/articles/app-model-recipe-site-provisioning.md)
- Guidance articles at [http://aka.ms/OfficeDevPnPGuidance](http://aka.ms/OfficeDevPnPGuidance "Guidance Articles")
- References in MSDN at [http://aka.ms/OfficeDevPnPMSDN](http://aka.ms/OfficeDevPnPMSDN "References in MSDN")
- Videos at [http://aka.ms/OfficeDevPnPVideos](http://aka.ms/OfficeDevPnPVideos "Videos")

Related PnP samples
===================

- [Core.CreateContentTypes (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/dev/Samples/Core.CreateContentTypes)
- [Core.ContentTypesAndFields (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/dev/Scenarios/Core.ContentTypesAndFields)
- [Core.CreateDocumentContentType (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/dev/Samples/Core.CreateDocumentContentType)
- [Branding.DisplayTemplates (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/master/Samples/Branding.DisplayTemplates)
- [Core.DataStorageModels (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/master/Samples/Core.DataStorageModels)
- Samples and content at https://github.com/OfficeDev/PnP

Applies to
==========
- Office 365 Multi Tenant (MT)
- Office 365 Dedicated (D) *partly*
- SharePoint 2013 on-premises – *partly*

*Patterns for dedicated and on-premises are identical with app model techniques, but there are differences on the possible technologies that can be used.*

Author
------
Todd Baginski (Canviz LLC) - [@toddbaginski](https://twitter.com/toddbaginski)

Version history
---------------
Version  | Date | Comments | Author
---------| -----| ---------| ------
0.1  | April 2, 2015 | Initial draft | Todd Baginski (Canviz LLC)
0.2  | April 5, 2015 | Trimmed article and updated content | Todd Baginski (Canviz LLC)
