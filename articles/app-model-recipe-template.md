# App model recipe - Themes #

App model recipe - Themes
=========================

###Summary###

Summary
-------

OneDrive for Business sites can be customized in Office 365 or with app model in general, based on company requirements. Actual techniques to perform this customization are different than in the on-premises, since only app model techniques can be used. This page contains details on the actual patterns which can be used with app model to customize OneDrive for Business sites.

When Vesa and I sync on each article I can take notes to assemble this summary.  I think it would be a good idea to sync on a series of articles before we start them to gather this info.

- Need to “Provide context and short introduction how the capability was done using FTC”
- Summary is really important to keep small and crisp, so that we get the context of the article. There's really no good example of this unfortunately.

# Why would you customize OneDrive for Business sites? #

This section contains the following information:
- Guidelines
	+ Sub bullet
- Summary
- Example

# Challenge with applying OneDrive for Business site customizations? #

Let’s start with defining what is the challenge and what are we trying to solve here. Technically each OneDrive for Business site is currently using identical architecture as what the personal or my sites used back in SharePoint 2007 or 2010 version. This means that technically each OneDrive for Business site is their own site collection and we do not have any centralized location to apply branding or any other customizations.

![](media/Recipes/Themes/agenda.jpg)

When Vesa and I sync on each article I can take notes to assemble the challenges.  I think it would be a good idea to sync on a series of articles before we start them to gather this info.

This section contains the following information:
- Challenges
- Different options for applying customizations

In practice we do have four different mechanisms to apply centralized customizations to OD4B sites in the Office 365. You could also consider manual option as the fifth one, but in the case of having hundreds or thousands of OD4B sites, using manual options is not really a realistic option. Here’s the different options we have.

1.	Office 365 suite level s ettings (Office 365 themes and other settings)
2.	Hidden app part with user context
3.	Pre-create and apply configuration
4.	Remote timer job based on user profile updates

Each of the options have advantages and disadvantages in them and the right option depends on your detailed business requirements. Some of the settings you can also apply from the Office 365 suite level, but often you would be looking for some more specifics, so actual customizations are needed. It obviously all comes down on exact requirements and business case analyses on their impact on short and long term.

When Vesa and I sync on each article I can take notes to assemble the options.  I think it would be a good idea to sync on a series of articles before we start them to gather this info.

This section contains the following information:

- Options
- Office 365 suite level settings

Office 365 is much more than just SharePoint, like you know. You can find more and more additional services which are not based on even the SharePoint architecture, like Delve, Yammer and many upcoming services. This means that the enterprise branding and configuration is not just about controlling what we have in the SharePoint sites, rather we should be thinking the overall end user experience and how we provide consistent configurations cross different services.

Classic example of these enterprise requirements is branding and for that we have already Office 365 theming introduced, which can be used to control some level of branding. We have also other upcoming features, which will help to control your site governance and other settings, from centralized location outside of the site collection settings, like the upcoming Compliance Center for Office 365, which is currently listed in the roadmap of the Office 365.

Following picture shows the different settings right now for the Office 365 theming, which will be then applied cross all Office 365 services.
 
Since by default Office 365 theme settings are for controlling OD4B site suite bar, you will most likely be using this options together with other options to ensure that you can provide at least the right branding elements cross your OD4B sites. Notice that when you change for example Office 365 theme settings in Office 365 admin tool, it does take a quite a long time to get the settings applied for OD4B sites, so be patience.

When Vesa and I sync on each article I can take notes to assemble the details about the options.  I think it would be a good idea to sync on a series of articles before we start them to gather this info.

This section contains the following information:

- Describe the option
- Include a diagram if it makes sense
- Show an example of when this option works well
- Point out any technical notes about this option

Related links
=============

•	Customizing OneDrive for Business sites with app model (MSDN blog article)
•	For each sample I can try my best to hunt them down.  When Vesa and I sync on each article he can let me know if I missed any.  I think it would be a good idea to sync on a series of articles before we start them to gather this info.
- Guidance articles at http://aka.ms/OfficeDevPnPGuidance
- References in MSDN at http://aka.ms/OfficeDevPnPMSDN 
- Videos at [http://aka.ms/OfficeDevPnPVideos](http://aka.ms/OfficeDevPnPVideos "Videos")

Related PnP samples
===================

•	Customizing OD4B sites using Async pattern
•	Classic app part and sync process for OD4B site customization
•	Pre-create OD4B sites for users
•	For each sample I can try my best to hunt them down.  When Vesa and I sync on each article he can let me know if I missed any.  I think it would be a good idea to sync on a series of articles before we start them to gather this info.
•	Samples and content at http://aka.ms/OfficeDevPnP
Applies to
==========
•	Office 365 Multi Tenant (MT)
•	Office 365 Dedicated (D) - partly
•	SharePoint 2013 on-premises – partly
•	Need to know all the possible choices we can have here and the exact names for them.
Patterns for Dedicated and on-premises are identical with app model techniques, but there are differences on the possible technologies which can be used.
Are there any other standard notes like this we might use across articles?
Author
======
Todd Baginski (Canviz LLC) - @toddbaginski
Version history
===============
Version	Date	Comments
1.0	January 2nd, 2015	Initial release

### Related links ###
-  [Customizing OneDrive for Business sites with app model (MSDN blog article)](http://blogs.msdn.com/b/vesku/archive/2015/01/01/customizing-onedrive-for-business-sites-with-app-model.aspx)

### Related PnP samples ###
-  [Customizing OD4B sites using Async pattern](#)
-  [Classic app part and sync process for OD4B site customization](https://github.com/OfficeDev/PnP/tree/master/Solutions/Provisioning.OneDrive)
-  [Pre-create OD4B sites for users](https://github.com/OfficeDev/PnP/tree/master/Samples/Provisioning.OneDriveProvisioning)

### Applies to ###
-  Office 365 Multi Tenant (MT)
-  Office 365 Dedicated (D) - *partly*
-  SharePoint 2013 on-premises - *partly*

*Patterns for Dedicated and on-premises are identical with app model techniques, but there are differences on the possible technologies which can be used.*

### Author
Todd Baginski (Canviz LLC) - [@toddbaginski](https://twitter.com/toddbaginski)

### Version history ###
Version  | Date | Comments
---------| -----| --------
1.0  | January 2nd, 2015 | Initial release | Vesa Juvonen (Microsoft)

