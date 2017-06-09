# CanvasControl Class
 Base class for a canvas control   

**Namespace:** [OfficeDevPnP.Core.Pages](OfficeDevPnP.Core.Pages.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;OfficeDevPnP.Core.Pages.CanvasControl  
&emsp;[OfficeDevPnP.Core.Pages.ClientSideText](OfficeDevPnP.Core.Pages.ClientSideText.md)  
&emsp;[OfficeDevPnP.Core.Pages.ClientSideWebPart](OfficeDevPnP.Core.Pages.ClientSideWebPart.md)  
## Syntax
```C#
public abstract class CanvasControl
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [CanvasControl()](OfficeDevPnP.Core.Pages.CanvasControl.ctor1.md) | Constructs the canvas control 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [CanvasControlData](OfficeDevPnP.Core.Pages.CanvasControl.CanvasControlData.md) | Value of the control's "data-sp-canvascontrol" attribute
| [ControlType](OfficeDevPnP.Core.Pages.CanvasControl.ControlType.md) | Type of the control: 3 is a text part, 4 is a client side web part
| [DataVersion](OfficeDevPnP.Core.Pages.CanvasControl.DataVersion.md) | The internal storage version used for this control
| [InstanceId](OfficeDevPnP.Core.Pages.CanvasControl.InstanceId.md) | Instance ID of the control
| [JsonControlData](OfficeDevPnP.Core.Pages.CanvasControl.JsonControlData.md) | Value of the control's "data-sp-controldata" attribute
| [Order](OfficeDevPnP.Core.Pages.CanvasControl.Order.md) | Order of the control in the control collection
| [Section](OfficeDevPnP.Core.Pages.CanvasControl.Section.md) | The [OfficeDevPnP.Core.Pages.CanvasSection](OfficeDevPnP.Core.Pages.CanvasSection.md) hosting this control 
| [Type](OfficeDevPnP.Core.Pages.CanvasControl.Type.md) | Type if the control ( [OfficeDevPnP.Core.Pages.ClientSideText](OfficeDevPnP.Core.Pages.ClientSideText.md) or T:OfficeDevPnP.Core.Pages.ClientSideWebPart) 
| [Zone](OfficeDevPnP.Core.Pages.CanvasControl.Zone.md) | The [OfficeDevPnP.Core.Pages.CanvasZone](OfficeDevPnP.Core.Pages.CanvasZone.md) hosting this control 
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Delete()](OfficeDevPnP.Core.Pages.CanvasControl.19cb6464.md) | Removes the control from the page
| [GetType(String)](OfficeDevPnP.Core.Pages.CanvasControl.c4f3d927.md) | Receives "data-sp-controldata" content and detects the type of the control
| [ToHtml(Int32)](OfficeDevPnP.Core.Pages.CanvasControl.bfd4198d.md) | Converts a control object to it's html representation
## See also
- [OfficeDevPnP.Core.Pages.CanvasSection](OfficeDevPnP.Core.Pages.CanvasSection.md)
- [OfficeDevPnP.Core.Pages.ClientSideText](OfficeDevPnP.Core.Pages.ClientSideText.md)
- [OfficeDevPnP.Core.Pages.ClientSideWebPart](OfficeDevPnP.Core.Pages.ClientSideWebPart.md)
- [OfficeDevPnP.Core.Pages.CanvasZone](OfficeDevPnP.Core.Pages.CanvasZone.md)
- [OfficeDevPnP.Core.Pages](OfficeDevPnP.Core.Pages.md)
