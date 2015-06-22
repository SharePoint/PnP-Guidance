SharePoint Add-in Recipe - Search Configuration
===============================================

Summary
-------

The approach you take to configure search is different in the new SharePoint Add-in model than it was with Full Trust Code.  In a typical Full Trust Code (FTC) / Farm Solution scenario, the SharePoint Server Side Object Model was used to configure search, and deployed via SharePoint Solutions.

In an SharePoint Add-in model scenario, you use the SharePoint Client Side Object Model (CSOM) or REST API to configure search. This pattern is commonly referred to as the *remote provisioning pattern*.

High Level Guidelines
---------------------

As a rule of a thumb, we would like to provide the following high level guidelines to configure search in the new SharePoint Add-in model.

- Use the SharePoint Client Side Object Model (CSOM) API to configure search whenever possible by importing and exporting search configuration settings.
- Not all search configuration settings are currently available via the SharePoint CSOM API.
	+ See the [Export and import customized search configuration settings in SharePoint Server 2013 (TechNet Article)](https://technet.microsoft.com/en-us/library/jj871675.aspx#BKMK_2) for a list of search configuration settings that can be exported and imported.
- The SharePoint REST API is not capable (at this time) of importing or exporting search configuration settings.

**Getting Started**

The following sample demonstrates how to import and export search settings between SharePoint tenants, site collections and sites.

- [Core.SearchSettingsPortability (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/master/Samples/Core.SearchSettingsPortability)

Related links
=============

- Guidance articles at [http://aka.ms/OfficeDevPnPGuidance](http://aka.ms/OfficeDevPnPGuidance "Guidance Articles")
- References in MSDN at [http://aka.ms/OfficeDevPnPMSDN](http://aka.ms/OfficeDevPnPMSDN "References in MSDN")
- Videos at [http://aka.ms/OfficeDevPnPVideos](http://aka.ms/OfficeDevPnPVideos "Videos")

Related PnP samples
===================

- [Core.SearchSettingsPortability (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/master/Samples/Core.SearchSettingsPortability)
- Samples and content at [http://aka.ms/OfficeDevPnP](http://aka.ms/OfficeDevPnP)

Applies to
==========
- Office 365 Multi Tenant (MT)
- Office 365 Dedicated (D)
- SharePoint 2013 on-premises

Author
------
Todd Baginski (Canviz LLC) - [@toddbaginski](https://twitter.com/toddbaginski)

Version history
---------------
Version  | Date | Comments | Author
---------| -----| ---------| ------
0.1  | June 22, 2015 | Initial draft | Todd Baginski (Canviz LLC)
