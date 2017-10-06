# ClientSideWebPart Class
This class is used to instantiate controls of type 3 (= client side web parts). Using this class you can instantiate a control and add it on a  [OfficeDevPnP.Core.Pages.ClientSidePage](OfficeDevPnP.Core.Pages.ClientSidePage.md)   

**Namespace:** [OfficeDevPnP.Core.Pages](OfficeDevPnP.Core.Pages.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Pages.CanvasControl](OfficeDevPnP.Core.Pages.CanvasControl.md)  
## Syntax
```C#
public class ClientSideWebPart: CanvasControl
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [ClientSideWebPart()](OfficeDevPnP.Core.Pages.ClientSideWebPart.ctor1.md) | Instantiates client side web part from scratch. 
| [ClientSideWebPart(ClientSideComponent)](OfficeDevPnP.Core.Pages.ClientSideWebPart.ctor2.md) | This class is used to instantiate controls of type 3 (= client side web parts). Using this class you can instantiate a control and add it on a [OfficeDevPnP.Core.Pages.ClientSidePage](OfficeDevPnP.Core.Pages.ClientSidePage.md) 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [Description](OfficeDevPnP.Core.Pages.ClientSideWebPart.Description.md) | Description of the web part
| [HtmlProperties](OfficeDevPnP.Core.Pages.ClientSideWebPart.HtmlProperties.md) | Value of the "data-sp-htmlproperties" attribute
| [HtmlPropertiesData](OfficeDevPnP.Core.Pages.ClientSideWebPart.HtmlPropertiesData.md) | Value of the "data-sp-htmlproperties" element
| [JsonWebPartData](OfficeDevPnP.Core.Pages.ClientSideWebPart.JsonWebPartData.md) | Value of the "data-sp-webpartdata" attribute
| [Properties](OfficeDevPnP.Core.Pages.ClientSideWebPart.Properties.md) |  Web properties as configurable Newtonsoft.Json.Linq.JObject 
| [PropertiesJson](OfficeDevPnP.Core.Pages.ClientSideWebPart.PropertiesJson.md) | Json serialized web part properties
| [SpControlData](OfficeDevPnP.Core.Pages.ClientSideWebPart.SpControlData.md) | Value of the "data-sp-controldata" attribute
| [Title](OfficeDevPnP.Core.Pages.ClientSideWebPart.Title.md) | Title of the web part
| [Type](OfficeDevPnP.Core.Pages.ClientSideWebPart.Type.md) | Return [OfficeDevPnP.Core.Pages.ClientSideWebPart.Type](OfficeDevPnP.Core.Pages.ClientSideWebPart.Type.md) of the client side web part 
| [WebPartData](OfficeDevPnP.Core.Pages.ClientSideWebPart.WebPartData.md) | Value of the "data-sp-webpart" attribute
| [WebPartId](OfficeDevPnP.Core.Pages.ClientSideWebPart.WebPartId.md) | ID of the client side web part
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Import(ClientSideComponent, Func&lt;String, String&gt;)](OfficeDevPnP.Core.Pages.ClientSideWebPart.587fffcf.md) | Imports a [OfficeDevPnP.Core.Pages.ClientSideComponent](OfficeDevPnP.Core.Pages.ClientSideComponent.md) to use it as base for configuring the client side web part instance 
| [ToHtml(Single)](OfficeDevPnP.Core.Pages.ClientSideWebPart.5d8c1207.md) | Returns a HTML representation of the client side web part
## See also
- [OfficeDevPnP.Core.Pages.ClientSidePage](OfficeDevPnP.Core.Pages.ClientSidePage.md)
- Newtonsoft.Json.Linq.JObject
- [OfficeDevPnP.Core.Pages.ClientSideWebPart.Type](OfficeDevPnP.Core.Pages.ClientSideWebPart.Type.md)
- [OfficeDevPnP.Core.Pages.ClientSideComponent](OfficeDevPnP.Core.Pages.ClientSideComponent.md)
- [OfficeDevPnP.Core.Pages](OfficeDevPnP.Core.Pages.md)
