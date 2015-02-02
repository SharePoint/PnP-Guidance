# CSOM releases and new capabilities #

### Summary ###
There have been significant changes on the Client Side Object Model (CSOM) capabilities after the initial release of the SharePoint 2013. This page is listing all the provided updates and is referencing specific samples for each of the updates. 

We will keep on updating this page based on the new capabilities released to cloud or to on-premises CSOM packages.

- Latest cloud CSOM re-distributable can be downloded from Microsoft download center using [aka.ms/spocsom](http://aka.ms/spocsom) address.

# Adding secondary site collection administrator to site collection #
Add secondary administrator to site collection.

- New public property Microsoft.SharePoint.Client.Site.SecondaryContact

### Platforms ###
On-Premises | Office 365
---------| ----------
2014 December CU  | -

### Related PnP samples ###
- 

### Related links ###
-  [Latest API updates in Client Side Object Model (Dec 2014 CU for SP2013)](http://blogs.msdn.com/b/vesku/archive/2014/12/15/latest-api-updates-in-client-side-object-model-dec-2014-cu-for-sp2013.aspx)

# Language settings in site level #
Control language settings in site level level.

- New public method Microsoft.SharePoint.Client.Web.AddSupportedUILanguage()
- New public method Microsoft.SharePoint.Client.Web.RemoveSupportedUILanguage()

*Update on 20th of Dec  - Adding additional language to web has unfortunately a bug and it does not work unless site has already one or more additional languages set, which means that this API does not really usable until this bug is fixed. This will be fixed for future releases and to redistributable version of the CSOM package*

### Platforms ###
On-Premises | Office 365
---------| ----------
2014 December CU  | -

### Related PnP samples ###
- [
Control regional and language settings using CSOM](https://github.com/OfficeDev/PnP/tree/master/Samples/Core.Settings.LocaleAndLanguage)

### Related links ###
-  [Latest API updates in Client Side Object Model (Dec 2014 CU for SP2013)](http://blogs.msdn.com/b/vesku/archive/2014/12/15/latest-api-updates-in-client-side-object-model-dec-2014-cu-for-sp2013.aspx)

# Regional settings in site level #
Control regional settings in site level level.

- New setter for public property Microsoft.SharePoint.Client.RegionalSettings.LocaleId
- New public method Microsoft.SharePoint.Client.RegionalSettings.Update()
  - You can access regional settings object from Microsoft.SharePoint.Client.Web.RegionalSettings property

### Platforms ###
On-Premises | Office 365
---------| ----------
2014 December CU  | -

### Related PnP samples ###
- [
Control regional and language settings using CSOM](https://github.com/OfficeDev/PnP/tree/master/Samples/Core.Settings.LocaleAndLanguage)

### Related links ###
-  [Latest API updates in Client Side Object Model (Dec 2014 CU for SP2013)](http://blogs.msdn.com/b/vesku/archive/2014/12/15/latest-api-updates-in-client-side-object-model-dec-2014-cu-for-sp2013.aspx)

# Version settings from list level #
Control additional version settings in list level.

- New public property Microsoft.SharePoint.Client.List.MajorVersionLimit
- New public property Microsoft.SharePoint.Client.List.MajorWithMinorVersionsLimit

### Platforms ###
On-Premises | Office 365
---------| ----------
2014 December CU  | -

### Related PnP samples ###
- 

### Related links ###
-  [Latest API updates in Client Side Object Model (Dec 2014 CU for SP2013)](http://blogs.msdn.com/b/vesku/archive/2014/12/15/latest-api-updates-in-client-side-object-model-dec-2014-cu-for-sp2013.aspx)

# Auditing settings #
Manipulate auditing settings in the site collection level.

- New public property Microsoft.SharePoint.Client.Site.Audit
- New public property Microsoft.SharePoint.Client.Site.AuditLogTrimmingRetention
- New public property Microsoft.SharePoint.Client.Site.TrimAuditLog
- New Class Microsoft.SharePoint.Client.Audit
- New Enum Microsoft.SharePoint.Client.AuditMaskType
- New Class Microsoft.SharePoint.Client.AuditPropertyNames

### Platforms ###
On-Premises | Office 365
---------| ----------
2014 December CU  | -

### Related PnP samples ###
- [
Control auditing settings in site collection using CSOM, Core.Settings.Audit  ](https://github.com/OfficeDev/PnP/tree/master/Samples/Core.Settings.Audit)

### Related links ###
-  [Latest API updates in Client Side Object Model (Dec 2014 CU for SP2013)](http://blogs.msdn.com/b/vesku/archive/2014/12/15/latest-api-updates-in-client-side-object-model-dec-2014-cu-for-sp2013.aspx)

# Edit user profile properties using CSOM #
Update user profile properties using CSOM APIs.

### Platforms ###
On-Premises | Office 365
---------| ----------
-  | Supported

### Related PnP samples ###
- [User profile manipulation using CSOM, UserProfile.Manipulation.CSOM  ](https://github.com/OfficeDev/PnP/tree/master/Samples/UserProfile.Manipulation.CSOM)
- [
User profile manipulation using CSOM, UserProfile.Manipulation.CSOM.Console  ](https://github.com/OfficeDev/PnP/tree/master/Samples/UserProfile.Manipulation.CSOM.Console)

### Related links ###
-  [SharePoint user profile properties now writable with CSOM](http://blogs.msdn.com/b/vesku/archive/2014/11/07/sharepoint-user-profile-properties-now-writable-with-csom.aspx)


# Provisioning site collections using SP App model in on-premises with just CSOM #
Site collection provisioning support added also to on-premises. This capability existed for Office 365 already previously, but was added later to the on-premises deployments

### Platforms ###
On-Premises | Office 365
---------| ----------
2014 April CU  | Supported

### Related PnP samples ###
- [Site collection provisioning in on-premises or Dedicated using CSOM, Provisioning.SiteCol.OnPrem ](https://github.com/OfficeDev/PnP/tree/master/Samples/Provisioning.SiteCol.OnPrem)
- [Asynchronious provisioning of site collections in on-premises, Provisioning.OnPrem.Async ](https://github.com/OfficeDev/PnP/tree/master/Samples/Provisioning.OnPrem.Async)

### Related links ###
-  [Provisioning site collections using SP App model in on-premises with just CSOM](http://blogs.msdn.com/b/vesku/archive/2014/06/09/provisioning-site-collections-using-sp-app-model-in-on-premises-with-just-csom.aspx)


# Multi-lingual content types, site columns and other site elements #
Add multilingual support for content types, site columns and other site elements using CSOM.

### Platforms ###
On-Premises | Office 365
---------| ----------
- | Supported

### Related PnP samples ###
- [Fields and Content Types, Core.ContentTypesAndFields](https://github.com/OfficeDev/PnP/tree/master/Scenarios/Core.ContentTypesAndFields)

### Related links ###
-  [Office365 – Multilingual content types, site columns and other site elements](http://blogs.msdn.com/b/vesku/archive/2014/03/20/office365-multilingual-content-types-site-columns-and-site-other-elements.aspx)


# Create content types using specific IDs #
Create content types using CSOM with support of defining the ID property for the content type.

### Platforms ###
On-Premises | Office 365
---------| ----------
SP2013 SP1 | Supported

### Related PnP samples ###
-  [
Creating Content Types, Core.CreateContentTypes](https://github.com/OfficeDev/PnP/tree/master/Samples/Core.CreateContentTypes)
- [Fields and Content Types, Core.ContentTypesAndFields](https://github.com/OfficeDev/PnP/tree/master/Scenarios/Core.ContentTypesAndFields)
- [
Create fields and content types based on element XML, Core.XMLBasedFieldsAndContentTypes](https://github.com/OfficeDev/PnP/tree/master/Scenarios/Core.XMLBasedFieldsAndContentTypes)

### Related links ###
-  [FTC to CAM – Create Content Types with specific IDs using CSOM](http://blogs.msdn.com/b/vesku/archive/2014/02/28/ftc-to-cam-create-content-types-with-specific-ids-using-csom.aspx)



----------

### Related links ###
*Referenced in specific chapters, not here*

### Related PnP samples ###
*Referenced in specific chapters, not here*

### Applies to ###
-  Office 365 Multi Tenant (MT)
-  Office 365 Dedicated (D)
-  SharePoint 2013 on-premises


### Author
Vesa Juvonen (Microsoft) - [@vesajuvonen](https://twitter.com/VesaJuvonen)

### Version history ###
Version  | Date | Author  
---------| -----| ------ 
1.0  | February 2nd 2015 | Initial release 


