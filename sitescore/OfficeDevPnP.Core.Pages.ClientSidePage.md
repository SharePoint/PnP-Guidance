# ClientSidePage Class
 Represents a modern client side page with all it's contents   

**Namespace:** [OfficeDevPnP.Core.Pages](OfficeDevPnP.Core.Pages.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public class ClientSidePage
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [ClientSidePage(ClientSidePageLayoutType)](OfficeDevPnP.Core.Pages.ClientSidePage.ctor1.md) | Constructs ClientSidePage class 
| [ClientSidePage(ClientContext, ClientSidePageLayoutType)](OfficeDevPnP.Core.Pages.ClientSidePage.ctor2.md) |  Represents a modern client side page with all it's contents 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [CommentsDisabled](OfficeDevPnP.Core.Pages.ClientSidePage.CommentsDisabled.md) | Does this page have comments disabled
| [Context](OfficeDevPnP.Core.Pages.ClientSidePage.Context.md) | ClientContext object that will be used to read and write to SharePoint
| [Controls](OfficeDevPnP.Core.Pages.ClientSidePage.Controls.md) | Collection of all control that exist on this client side page
| [DefaultZone](OfficeDevPnP.Core.Pages.ClientSidePage.DefaultZone.md) | The default zone of the client side page
| [KeepDefaultWebParts](OfficeDevPnP.Core.Pages.ClientSidePage.KeepDefaultWebParts.md) | When a page of type Home is created you can opt to only keep the default client side web parts by setting this to true. This also is a way to reset your home page back the the stock one.
| [LayoutType](OfficeDevPnP.Core.Pages.ClientSidePage.LayoutType.md) | Layout type of the client side page
| [PageListItem](OfficeDevPnP.Core.Pages.ClientSidePage.PageListItem.md) | The SharePoint list item of the saved/loaded page
| [PagesLibrary](OfficeDevPnP.Core.Pages.ClientSidePage.PagesLibrary.md) | The site relative path to SitePages library
| [PageTitle](OfficeDevPnP.Core.Pages.ClientSidePage.PageTitle.md) | Title of the client side page
| [Zones](OfficeDevPnP.Core.Pages.ClientSidePage.Zones.md) | Collection of Zones that exist on this client side page
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [AddControl(CanvasControl)](OfficeDevPnP.Core.Pages.ClientSidePage.6602702a.md) | Adds a new control to your client side page using the default [OfficeDevPnP.Core.Pages.CanvasZone](OfficeDevPnP.Core.Pages.CanvasZone.md) 
| [AddControl(CanvasControl, Int32)](OfficeDevPnP.Core.Pages.ClientSidePage.25bd9616.md) | Adds a new control to your client side page using the default [OfficeDevPnP.Core.Pages.CanvasZone](OfficeDevPnP.Core.Pages.CanvasZone.md) using a given order 
| [AddControl(CanvasControl, CanvasZone)](OfficeDevPnP.Core.Pages.ClientSidePage.38a1e3b9.md) | Adds a new control to your client side page in the given zone
| [AddControl(CanvasControl, CanvasZone, Int32)](OfficeDevPnP.Core.Pages.ClientSidePage.cc95a39b.md) | Adds a new control to your client side page in the given zone with a given order
| [AddControl(CanvasControl, CanvasSection)](OfficeDevPnP.Core.Pages.ClientSidePage.df7f51fa.md) | Adds a new control to your client side page in the given section
| [AddControl(CanvasControl, CanvasSection, Int32)](OfficeDevPnP.Core.Pages.ClientSidePage.721601f8.md) | Adds a new control to your client side page in the given section with a given order
| [AddZone(CanvasZoneTemplate, Int32)](OfficeDevPnP.Core.Pages.ClientSidePage.f2e77f52.md) | Adds a new zone to your client side page
| [AddZone(CanvasZone)](OfficeDevPnP.Core.Pages.ClientSidePage.4617fca2.md) | Adds a new zone to your client side page
| [AddZone(CanvasZone, Single)](OfficeDevPnP.Core.Pages.ClientSidePage.3e5fb18e.md) | Adds a new zone to your client side page with a given order
| [AvailableClientSideComponents()](OfficeDevPnP.Core.Pages.ClientSidePage.b6ddde41.md) | Gets a list of available client side web parts to use
| [AvailableClientSideComponents(DefaultClientSideWebParts)](OfficeDevPnP.Core.Pages.ClientSidePage.6beeff0e.md) | Gets an out of the box, default, client side web parts to use
| [AvailableClientSideComponents(String)](OfficeDevPnP.Core.Pages.ClientSidePage.fd6341ca.md) | Gets a list of available client side web parts to use having a given name
| [ClientSideWebPartEnumToName(DefaultClientSideWebParts)](OfficeDevPnP.Core.Pages.ClientSidePage.6de96379.md) | Return the name (=guid) for a given first party out of the box web part
| [Delete()](OfficeDevPnP.Core.Pages.ClientSidePage.19cb6464.md) | Deletes a control from a page
| [DemoteNewsArticle()](OfficeDevPnP.Core.Pages.ClientSidePage.1f2c0049.md) |  Demotes an client side F:OfficeDevPnP.Core.Pages.ClientSidePageLayoutType.Article news page as a regular client side page 
| [DisableComments()](OfficeDevPnP.Core.Pages.ClientSidePage.4efc25e7.md) | Disable commenting on this page
| [EnableComments()](OfficeDevPnP.Core.Pages.ClientSidePage.4b17fc50.md) | Enable commenting on this page
| [FromHtml(String)](OfficeDevPnP.Core.Pages.ClientSidePage.5145f098.md) | Instantiate a [OfficeDevPnP.Core.Pages.ClientSidePage](OfficeDevPnP.Core.Pages.ClientSidePage.md) from a html fragment 
| [InstantiateDefaultWebPart(DefaultClientSideWebParts)](OfficeDevPnP.Core.Pages.ClientSidePage.c91a53c3.md) | Creates an instance of an out of the box (default, first party) client side web part
| [Load(ClientContext, String)](OfficeDevPnP.Core.Pages.ClientSidePage.83cd9dec.md) | Loads an existint SharePoint client side page
| [PromoteAsHomePage()](OfficeDevPnP.Core.Pages.ClientSidePage.f5e3825.md) | Sets the current [OfficeDevPnP.Core.Pages.ClientSidePage](OfficeDevPnP.Core.Pages.ClientSidePage.md) as home page for the current site 
| [PromoteAsNewsArticle()](OfficeDevPnP.Core.Pages.ClientSidePage.a39307d1.md) |  Promotes a regular F:OfficeDevPnP.Core.Pages.ClientSidePageLayoutType.Article client side page as a news page 
| [Publish()](OfficeDevPnP.Core.Pages.ClientSidePage.cfed9fc3.md) | Publishes a client side page
| [Publish(String)](OfficeDevPnP.Core.Pages.ClientSidePage.4e0728bf.md) | Publishes a client side page
| [Save(String)](OfficeDevPnP.Core.Pages.ClientSidePage.679ae7d1.md) | Persists the current [OfficeDevPnP.Core.Pages.ClientSidePage](OfficeDevPnP.Core.Pages.ClientSidePage.md) instance as a client side page in SharePoint 
| [ToHtml()](OfficeDevPnP.Core.Pages.ClientSidePage.7c2b006f.md) | Returns the html representation of this client side page. This is the content that will be persisted in the [OfficeDevPnP.Core.Pages.ClientSidePage.PageListItem](OfficeDevPnP.Core.Pages.ClientSidePage.PageListItem.md) list item 
## See also
- [OfficeDevPnP.Core.Pages.ClientSidePageLayoutType](OfficeDevPnP.Core.Pages.ClientSidePageLayoutType.md)
- Microsoft.SharePoint.Client.ClientContext
- [OfficeDevPnP.Core.Pages.CanvasZone](OfficeDevPnP.Core.Pages.CanvasZone.md)
- [OfficeDevPnP.Core.Pages.CanvasControl](OfficeDevPnP.Core.Pages.CanvasControl.md)
- [OfficeDevPnP.Core.Pages.CanvasZone.DefaultSection](OfficeDevPnP.Core.Pages.CanvasZone.DefaultSection.md)
- [OfficeDevPnP.Core.Pages.CanvasSection](OfficeDevPnP.Core.Pages.CanvasSection.md)
- [OfficeDevPnP.Core.Pages.CanvasZoneTemplate](OfficeDevPnP.Core.Pages.CanvasZoneTemplate.md)
- [OfficeDevPnP.Core.Pages.ClientSideComponent](OfficeDevPnP.Core.Pages.ClientSideComponent.md)
- F:OfficeDevPnP.Core.Pages.ClientSidePageLayoutType.Article
- [OfficeDevPnP.Core.Pages.ClientSidePage](OfficeDevPnP.Core.Pages.ClientSidePage.md)
- [OfficeDevPnP.Core.Pages.ClientSideWebPart](OfficeDevPnP.Core.Pages.ClientSideWebPart.md)
- [OfficeDevPnP.Core.Pages.ClientSidePage.PageListItem](OfficeDevPnP.Core.Pages.ClientSidePage.PageListItem.md)
- [OfficeDevPnP.Core.Pages](OfficeDevPnP.Core.Pages.md)
