# CommunicationSiteCollectionCreationInformation Class
  

**Namespace:** [OfficeDevPnP.Core.Sites](OfficeDevPnP.Core.Sites.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public class CommunicationSiteCollectionCreationInformation
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [CommunicationSiteCollectionCreationInformation()](OfficeDevPnP.Core.Sites.CommunicationSiteCollectionCreationInformation.ctor1.md) |  
| [CommunicationSiteCollectionCreationInformation(String, String, String)](OfficeDevPnP.Core.Sites.CommunicationSiteCollectionCreationInformation.ctor2.md) |  
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [AllowFileSharingForGuestUsers](OfficeDevPnP.Core.Sites.CommunicationSiteCollectionCreationInformation.AllowFileSharingForGuestUsers.md) | If set to true, file sharing for guest users will be allowed.
| [Classification](OfficeDevPnP.Core.Sites.CommunicationSiteCollectionCreationInformation.Classification.md) | The Site classification to use. For instance 'Contoso Classified'. See https://www.youtube.com/watch?v=E-8Z2ggHcS0 for more information
| [Description](OfficeDevPnP.Core.Sites.CommunicationSiteCollectionCreationInformation.Description.md) | The description to use for the site.
| [Lcid](OfficeDevPnP.Core.Sites.CommunicationSiteCollectionCreationInformation.Lcid.md) | The language to use for the site. If not specified will default to the language setting of the clientcontext.
| [Owner](OfficeDevPnP.Core.Sites.CommunicationSiteCollectionCreationInformation.Owner.md) | The owner of the site. Reserved for future use.
| [SiteDesign](OfficeDevPnP.Core.Sites.CommunicationSiteCollectionCreationInformation.SiteDesign.md) | The built-in site design to used. If both SiteDesignId and SiteDesign have been specified, the GUID specified as SiteDesignId will be used.
| [SiteDesignId](OfficeDevPnP.Core.Sites.CommunicationSiteCollectionCreationInformation.SiteDesignId.md) | The Guid of the site design to be used. If specified will override the SiteDesign property
| [Title](OfficeDevPnP.Core.Sites.CommunicationSiteCollectionCreationInformation.Title.md) | The title of the site to create
| [Url](OfficeDevPnP.Core.Sites.CommunicationSiteCollectionCreationInformation.Url.md) | The fully qualified url (e.g. https://yourtenant.sharepoint.com/sites/mysitecollection) of the site.
## See also
- [OfficeDevPnP.Core.Sites](OfficeDevPnP.Core.Sites.md)
