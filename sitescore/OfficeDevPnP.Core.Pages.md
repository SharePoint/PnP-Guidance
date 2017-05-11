# OfficeDevPnP.Core.Pages
## Classes
|**Class**|**Description**|
|:-----|:-----|
|[ClientSidePage](OfficeDevPnP.Core.Pages.ClientSidePage.md)|Represents a modern client side page with all it's contents|
|[CanvasZone](OfficeDevPnP.Core.Pages.CanvasZone.md)|Represents a zone on the canvas|
|[CanvasSection](OfficeDevPnP.Core.Pages.CanvasSection.md)|Represents a section in a canvas zone|
|[AvailableClientSideComponents](OfficeDevPnP.Core.Pages.AvailableClientSideComponents.md)|Class holding a collection of client side webparts (retrieved via the _api/web/GetClientSideWebParts REST call)|
|[ClientSideComponent](OfficeDevPnP.Core.Pages.ClientSideComponent.md)|Client side webpart object (retrieved via the _api/web/GetClientSideWebParts REST call)|
|[CanvasControl](OfficeDevPnP.Core.Pages.CanvasControl.md)|Base control|
|[ClientSideText](OfficeDevPnP.Core.Pages.ClientSideText.md)|Controls of type 4 ( = text control)|
|[ClientSideWebPart](OfficeDevPnP.Core.Pages.ClientSideWebPart.md)| This class is used to instantiate controls of type 3 (= client side web parts). Using this class you can instantiate a control and add it on a T:OfficeDevPnP.Core.Pages.ClientSidePage. |
|[ClientSideCanvasControlData](OfficeDevPnP.Core.Pages.ClientSideCanvasControlData.md)|Abstract base class representing the json control data that will be included in each client side control (de-)serialization (data-sp-controldata attribute)|
|[ClientSideTextControlData](OfficeDevPnP.Core.Pages.ClientSideTextControlData.md)|Control data for controls of type 4 (= text control)|
|[ClientSideWebPartControlData](OfficeDevPnP.Core.Pages.ClientSideWebPartControlData.md)|Control data for controls of type 3 (= client side web parts)|
|[ClientSideWebPartData](OfficeDevPnP.Core.Pages.ClientSideWebPartData.md)|Json web part data that will be included in each client side web part (de-)serialization (data-sp-webpartdata)|
## Enumerations
|**Enumeration**|**Description**|
|:-----|:-----|
|[DefaultClientSideWebParts](OfficeDevPnP.Core.Pages.DefaultClientSideWebParts.md)|List of possible OOB web parts|
|[CanvasZoneTemplate](OfficeDevPnP.Core.Pages.CanvasZoneTemplate.md)|The type of canvas being used|
