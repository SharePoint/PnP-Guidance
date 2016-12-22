# Customizing the "modern" experiences in SharePoint Online
SharePoint Online has started the gradual introduction of "modern" experiences cross the SharePoint service, which has a direct impact on the end user experience but also on the customization options that can be used. This article provides an overview of the "modern" experiences to get you started and there are links to articles containing all the customization options for each of the "modern" experiences.

There are numerous benefits in the "modern" experiences called out on referenced materials, but if you have specific customization requirements, you need to be aware of the currently supported options for customization.

>**Important:** 
We're not deprecating the "classic" experience, both "classic" and "modern" will coexist.

_**Applies to:** SharePoint Online_

## What are the "modern" experiences in SharePoint Online?
<a name="sectionSection0"> </a>
The modern experiences in SharePoint Online are:
- **Modern team sites**
- **Modern list and library experiences**
- **Modern site pages** 

"Modern" experiences are gradually released in SharePoint Online and you can control how they are taken into use from tenant or site level. If you have a lot of existing important customizations, you can defer taking new experiences into use until needed customizations scenarios can be enabled with them as well. 

We recommend using the following process for adopting to the "modern" experiences, if you have existing customizations which are business critical for your deployment:

1. **Readiness**: Understand the "modern" experiences, know what features they offer but equally important understand what's features are not (yet) available
2. **Assess**: Assess to what extend your current customizations can work in the "modern" experience. Also assess which of your sites do have customizations or features that will not work in the "modern" experiences, these sites and their customizations should be updated or need to stay in "classic". However all other sites should work fine using the "modern" experiences.
3. **Solution planning**: Plan the needed work on both custom solutions as sites to prepare them to be used with the "modern" experiences 
4. **Develop and test**: Apply the needed changes to your customizations and test them 
5. **Deploy**: Roll out the updated changes to your SharePoint Online environment

Here are the key scenarios currently supported by the "modern" experiences. We will be updating the list of supported scenarios whenever new capabilities are being introduced in SharePoint Online. 

|**Customization**|**Introduction to options**|
|:-----|:-----|
|Provisioning "modern" team sites|<p>"Modern" team sites can be provisioned by an end user but you can also create these sites programmatically which is explained in detail in this article.</p><p>[Provisioning modern team sites](modern-experience-customizations-provisioning-sites.md)</p>|
|Customizing "modern" team sites|<p>"Modern" team sites are sites which bring a fresh new responsive user experience to SharePoint Online, showing relevant information on the home page. Typically these sites also have a corresponding Office 365 Group associated. You can learn more about the customization options via below link.</p><p>[Customizing modern team sites](modern-experience-customizations-customize-sites.md)</p>|
|Customizing "modern" lists and libraries|<p>"Modern" lists  and document libraries bring a better user experience which is faster, more intuitive and responsive. This article focuses on the extensibility options, such as user custom actions and branding, which are supported for the "modern" library and list experiences. </p><p>[Customizing modern lists and libraries](modern-experience-customizations-customize-lists-and-libraries.md)</p>|
|Customizing "modern" site pages|<p>"Modern" team site pages are fast, easy to author and support rich multimedia content. And pages look great on any device, in a browser or from within the SharePoint mobile app. This article focuses on the extensibility options there are in the "modern" page experience</p><p>[Customizing modern site pages](modern-experience-customizations-customize-pages.md)</p>|

## Converting existing sites to "modern" team sites
<a name="convertingexisting"> </a>
Existing collaborations sites cannot, at least currently, be converted to "modern" team sites with associated Office 365 group. You can however start using "modern" experiences in the "classic" collaboration sites as well by enabling the new capabilities at tenant level and then modify the sites based on the functional requirements. 

"Modern" lists and library usage can be controlled from tenant, site, web and in list/library level. You can find more details on the available options in our [modern list and libraries](local://base_request.html/modern-experience-customizations-customize-lists-and-libraries.md) article.

By default "classic" SharePoint sites will also use "modern" pages for any newly added page and you do have the option to change the welcome page to be a "modern" page. Setting a new "modern" page for "classic" SharePoint site can be done programatically using CSOM or REST APIs. 

## SharePoint "modern" experiences support for on-premises
<a name="onpremisessupport"> </a>
The SharePoint "modern" experiences are currently not available for SharePoint on-premises. They are planned to, step by step, become available for SharePoint 2016 as part of upcoming feature packs.

## Additional resources
<a name="bk_addresources"> </a>

-  [Create connected SharePoint Online team sites in seconds](https://blogs.office.com/2016/11/08/create-connected-sharepoint-online-team-sites-in-seconds/)

-  [New capabilities in SharePoint Online team sites including integration with Office 365 groups](https://blogs.office.com/2016/08/31/new-capabilities-in-sharepoint-online-team-sites-including-integration-with-office-365-groups/)

-  [Turn scripting capabilities on or off](https://support.office.com/en-us/article/Turn-scripting-capabilities-on-or-off-1f2c515f-5d7e-448a-9fd7-835da935584f) - Notice that you cannot enable scripting capabilities in the "modern" team sites, but this article defines the features, which are affected when scripting is disabled
    
-  ["Modern" SharePoint lists are here - including integration with Microsoft Flow and PowerApps](https://blogs.office.com/2016/07/25/modern-sharepoint-lists-are-here-including-integration-with-microsoft-flow-and-powerapps/)

-  [Update on "Modern" Document Libraries and Extensibility](https://dev.office.com/blogs/update-on-modern-document-libraries-and-extensiblity)

-  [Switch the default experience for lists or document libraries from "modern" or "classic"](https://support.office.com/en-us/article/Switch-the-default-experience-for-lists-or-document-libraries-from-new-or-classic-66dac24b-4177-4775-bf50-3d267318caa9?ui=en-US&rs=en-US&ad=US)
