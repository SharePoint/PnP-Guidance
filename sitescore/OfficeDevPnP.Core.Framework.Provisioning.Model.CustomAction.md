# CustomAction Class
 Domain Object for custom actions associated with a SharePoint list, Web site, or subsite. 

 Domain Object for custom actions associated with a SharePoint list, Web site, or subsite.   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel](OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel.md)  
## Syntax
```C#
public class CustomAction: BaseModel, IEquatable<CustomAction>
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [CustomAction()](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.ctor1.md) |  Domain Object for custom actions associated with a SharePoint list, Web site, or subsite. Domain Object for custom actions associated with a SharePoint list, Web site, or subsite. 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [ClientSideComponentId](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.ClientSideComponentId.md) | Gets or sets a value for the ClientSideComponentId, if any
| [ClientSideComponentProperties](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.ClientSideComponentProperties.md) | Gets or sets a value for the ClientSideComponentProperties, if any
| [CommandUIExtension](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.CommandUIExtension.md) | 
| [Description](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.Description.md) | Gets or sets the description of the custom action.
| [Enabled](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.Enabled.md) | Gets or sets the Enabled property value.
| [Group](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.Group.md) | Gets or sets a value that specifies an implementation-specific value that determines the position of the custom action in the page.
| [ImageUrl](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.ImageUrl.md) | Gets or sets the URL of the image associated with the custom action.
| [Location](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.Location.md) | Gets or sets the location of the custom action. A string that contains the location; for example, Microsoft.SharePoint.SiteSettings.
| [Name](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.Name.md) | Gets or sets the name of the custom action.
| [RegistrationId](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.RegistrationId.md) | Gets or sets the RegistrationId of the custom action.
| [RegistrationType](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.RegistrationType.md) | Gets or sets the RegistrationType of the custom action.
| [Remove](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.Remove.md) | Gets or sets a value that specifies whether to Remove the CustomAction from the target
| [Rights](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.Rights.md) | Gets or sets the value that specifies the permissions needed for the custom action.
| [RightsValue](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.RightsValue.md) |  Gets or sets the value that specifies the permissions needed for the custom action. https://msdn.microsoft.com/en-us/library/office/microsoft.sharepoint.client.permissionkind.aspx
| [ScriptBlock](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.ScriptBlock.md) | Gets or sets the value that specifies the ECMAScript to be executed when the custom action is performed.
| [ScriptSrc](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.ScriptSrc.md) | Gets or sets a value that specifies the URI of a file which contains the ECMAScript to execute on the page
| [Sequence](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.Sequence.md) | Gets or sets the value that specifies an implementation-specific value that determines the order of the custom action that appears on the page.
| [Title](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.Title.md) | Gets or sets the display title of the custom action.
| [Url](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.Url.md) | Gets or sets the URL, URI, or ECMAScript (JScript, JavaScript) function associated with the action.
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Equals(Object)](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.3520ddbb.md) | Compares object with CustomAction
| [Equals(CustomAction)](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.41d3ef4c.md) | Compares CustomAction object based on CommandUIExtension, Description, Enabled, Group, ImageUrl, Location, Name, RegistrationId, RegistrationType, Remove, Rights, ScriptBlock, ScriptSrc, Sequence, Title and Url properties.
| [GetHashCode()](OfficeDevPnP.Core.Framework.Provisioning.Model.CustomAction.1c6872bd.md) | Gets the hash code
## See also
- [https://msdn.microsoft.com/en-us/library/office/microsoft.sharepoint.client.permissionkind.aspx](https://msdn.microsoft.com/en-us/library/office/microsoft.sharepoint.client.permissionkind.aspx)
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
