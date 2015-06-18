SharePoint Add-in model recipe - Modules
========================================

Summary
-------

The approach you take to deploy artifacts to a SharePoint environment is different in the new SharePoint Add-in model than it was with Full Trust Code.  In a typical Full Trust Code (FTC) / Farm Solution scenario, modules defined in declarative code were added to SharePoint features.  The modules included the list of artifacts to deploy to the SharePoint server.  The modules were added to SharePoint features and deployed via SharePoint Solutions.  Upon feature activation, the artifacts defined in the modules were deployed to the SharePoint environment.

In a SharePoint Add-in model scenario, the remote provisioning pattern is used to deploy artifacts to SharePoint environments.

Terminology
-----------

The term *artifacts* is referred to throughout this article.  Artifacts refers to items that are typically deployed to a SharePoint environment.  Artifacts typically include:

- JavaScript files
- CSS files
- Image files (.jpg, .gif, .png, etc.)
- Master Pages
- Page Layouts
- List Items

High Level Guidelines
---------------------

As a rule of a thumb, we would like to provide the following high level guidelines to deploy artifacts to SharePoint environments.

- Use the remote provisioning pattern (SharePoint Client Side Object Model and SharePoint REST API) to deploy artifacts to SharePoint environments.
- Do not use declarative code modules to deploy artifacts to SharePoint environments.

**Getting Started**

The following O365 PnP Code Samples and video demonstrate how to create a SharePoint Add-ins that use the remote provisioning pattern to deploy artifacts to a SharePoint environment.

  This sample demonstrates how to create a new folders in the Style Library and add JavaScript files and images to the new files.

- [Branding.ClientSideRendering (O365 PnP Code Sample)](https://github.com/OfficeDev/PnP/tree/master/Samples/Branding.ClientSideRendering)
	+ See the ***UploadJSFiles*** and the ***UploadFileToFolder*** methods in the [Default.aspx.cs class](https://github.com/OfficeDev/PnP/blob/master/Samples/Branding.ClientSideRendering/Branding.ClientSideRenderingWeb/Pages/Default.aspx.cs) for more details.

This sample demonstrates how to upload master pages, set master page meta data, and apply the master page to the site by setting the CustomMasterUrl property on the Web object.

- [Branding.ApplyBranding (O365 PnP Code Sample)](https://github.com/OfficeDev/PnP/tree/master/Samples/Branding.ApplyBranding)
	+ See the ***UploadPageLayout***, ***CreatePublishingPage***, and ***SetSupportCaseContent*** methods in the [BrandingHelper.cs class](https://github.com/OfficeDev/PnP/blob/master/Samples/Branding.ApplyBranding/Branding.ApplyBranding.Console/BrandingHelper.cs) for more details.
	+ Watch the [Applying Branding to SharePoint Sites with an App for SharePoint (Office 365 PnP Video)](https://channel9.msdn.com/Blogs/Office-365-Dev/Applying-Branding-to-SharePoint-Sites-with-an-App-for-SharePoint-Office-365-Developer-Patterns-and-P) for a walk through of this sample.

This sample demonstrates how to upload page layouts, create publishing pages, add Add-in Parts to pages.  It also demonstrates how to deploy list items to both the host web and the Add-in web.

- [Branding.ClientSideRendering (O365 PnP Code Sample)](https://github.com/OfficeDev/PnP/tree/master/Samples/Branding.ClientSideRendering)
	+ See the ***UploadPageLayout***, ***CreatePublishingPage***, and ***SetSupportCaseContent*** methods in the [Utils.cs class](https://github.com/OfficeDev/PnP/blob/master/Samples/Core.DataStorageModels/Core.DataStorageModelsWeb/Util/Util.cs) for more details about uploading page layouts, creating publishing pages, adding Add-in Parts to pages.
	+ See the ***FillHostWebSupportCasesToThreshold*** and the ***FillAppWebNotesListToThreshold*** methods in the [SharePointService.cs class](https://github.com/OfficeDev/PnP/blob/master/Samples/Core.DataStorageModels/Core.DataStorageModelsWeb/Services/SharePointService.cs) for more details about deploying list items to both the host web and the Add-in web.  
	+ ***Important note:*** The same host web and Add-in web approaches demonstrated in this sample may be applied to any type of artifact to deploy them to the appropriate location.
	
Related links
=============

- [Master Pages (SharePoint Add-in Recipe)](https://github.com/OfficeDev/PnP-Guidance/blob/master/articles/SharePoint-Add-In-Recipe-master-pages.md)
- Guidance articles at [http://aka.ms/OfficeDevPnPGuidance](http://aka.ms/OfficeDevPnPGuidance "Guidance Articles")
- References in MSDN at [http://aka.ms/OfficeDevPnPMSDN](http://aka.ms/OfficeDevPnPMSDN "References in MSDN")
- Videos at [http://aka.ms/OfficeDevPnPVideos](http://aka.ms/OfficeDevPnPVideos "Videos")

Related PnP samples
===================

- [Branding.ClientSideRendering (O365 PnP Code Sample)](https://github.com/OfficeDev/PnP/tree/master/Samples/Branding.ClientSideRendering)
- [Branding.ApplyBranding (O365 PnP Code Sample)](https://github.com/OfficeDev/PnP/tree/master/Samples/Branding.ApplyBranding)
- [Branding.ClientSideRendering (O365 PnP Code Sample)](https://github.com/OfficeDev/PnP/tree/master/Samples/Branding.ClientSideRendering)
- Samples and content at https://github.com/OfficeDev/PnP

Applies to
==========
- Office 365 Multi Tenant (MT)
- Office 365 Dedicated (D) *partly*
- SharePoint 2013 on-premises – *partly*

*Patterns for dedicated and on-premises are identical with SharePoint Add-in model techniques, but there are differences on the possible technologies that can be used.*

Author
------
Todd Baginski (Canviz LLC) - [@toddbaginski](https://twitter.com/toddbaginski)

Version history
---------------
Version  | Date | Comments | Author
---------| -----| ---------| ------
0.1  | June 18, 2015 | Initial draft | Todd Baginski (Canviz LLC)