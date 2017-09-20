# PageExtensions Class
 Class that holds all deprecated page and web part related operations 

 Class that handles all page and web part related operations   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class PageExtensions
```
## Extension Methods
|**Name**|**Description**|
|:-----|:-----|
| [AddClientSidePage(Web, String, Boolean)](Microsoft.SharePoint.Client.PageExtensions.6f33066a.md) | Adds a client side "modern" page to a "classic" or "modern" site
| [AddHtmlToWikiPage(Web, String, String, String)](Microsoft.SharePoint.Client.PageExtensions.6b3135f8.md) | Add html to a wiki style page
| [AddHtmlToWikiPage(Web, String, String)](Microsoft.SharePoint.Client.PageExtensions.eefb32ca.md) | Add HTML to a wiki page
| [AddHtmlToWikiPage(Web, String, String, String, Int32, Int32)](Microsoft.SharePoint.Client.PageExtensions.f106101.md) | Add a HTML fragment to a location on a wiki style page
| [AddHtmlToWikiPage(Web, String, String, Int32, Int32)](Microsoft.SharePoint.Client.PageExtensions.6162ae7f.md) | Add a HTML fragment to a location on a wiki style page
| [AddLayoutToWikiPage(Web, WikiPageLayout, String)](Microsoft.SharePoint.Client.PageExtensions.378f99ab.md) | Applies a layout to a wiki page
| [AddLayoutToWikiPage(Web, String, WikiPageLayout, String)](Microsoft.SharePoint.Client.PageExtensions.f1459c5d.md) | Applies a layout to a wiki page
| [AddNavigationFriendlyUrl(PublishingPage, Web, String, String, NavigationTermSetItem, Boolean, Boolean)](Microsoft.SharePoint.Client.PageExtensions.f1399c44.md) | Adds a user-friendly URL for a PublishingPage object.
| [AddWebPartToWebPartPage(Web, WebPartEntity, String)](Microsoft.SharePoint.Client.PageExtensions.1faef384.md) | Inserts a web part on a web part page
| [AddWebPartToWebPartPage(Web, String, WebPartEntity)](Microsoft.SharePoint.Client.PageExtensions.e7d82354.md) | Inserts a web part on a web part page
| [AddWebPartToWikiPage(Web, String, WebPartEntity, String, Int32, Int32, Boolean)](Microsoft.SharePoint.Client.PageExtensions.f8118ef.md) | Add web part to a wiki style page
| [AddWebPartToWikiPage(Web, String, WebPartEntity, Int32, Int32, Boolean)](Microsoft.SharePoint.Client.PageExtensions.83b57943.md) | Add web part to a wiki style page
| [AddWikiPage(Web, String, String)](Microsoft.SharePoint.Client.PageExtensions.43b33c77.md) | Adds a blank Wiki page to the site pages library
| [AddWikiPageByUrl(Web, String, String)](Microsoft.SharePoint.Client.PageExtensions.a5de1d3d.md) | Adds a wiki page by Url
| [DeleteWebPart(Web, String, String, String)](Microsoft.SharePoint.Client.PageExtensions.569afb87.md) | Deletes a web part from a page
| [DeleteWebPart(Web, String, String)](Microsoft.SharePoint.Client.PageExtensions.14c6ffe4.md) | Deletes a web part from a page
| [EnsureWikiPage(Web, String, String)](Microsoft.SharePoint.Client.PageExtensions.2efd9f8f.md) | Returns the Url for the requested wiki page, creates it if the pageis not yet available
| [GetWebPartProperties(Web, Guid, String)](Microsoft.SharePoint.Client.PageExtensions.4f627997.md) | Returns web part properties
| [GetWebParts(Web, String)](Microsoft.SharePoint.Client.PageExtensions.37813d52.md) | List the web parts on a page
| [GetWebPartXml(Web, Guid, String)](Microsoft.SharePoint.Client.PageExtensions.dfcbd0d1.md) | Gets XML string of a Webpart
| [GetWikiPageContent(Web, String)](Microsoft.SharePoint.Client.PageExtensions.bfdefefa.md) | Gets the HTML contents of a wiki page
| [LoadClientSidePage(Web, String)](Microsoft.SharePoint.Client.PageExtensions.398b8deb.md) | Loads a client side "modern" page
| [SetWebPartProperty(Web, String, String, Guid, String)](Microsoft.SharePoint.Client.PageExtensions.ca57f4e2.md) | Sets a web part property
| [SetWebPartProperty(Web, String, Int32, Guid, String)](Microsoft.SharePoint.Client.PageExtensions.da634517.md) | Sets a web part property
| [SetWebPartProperty(Web, String, Boolean, Guid, String)](Microsoft.SharePoint.Client.PageExtensions.76177fde.md) | Sets a web part property
## See also
- [OfficeDevPnP.Core.Pages.ClientSidePage](OfficeDevPnP.Core.Pages.ClientSidePage.md)
- System.ArgumentException
- System.ArgumentNullException
- Microsoft.SharePoint.Client.WebParts.WebPartDefinition
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)
