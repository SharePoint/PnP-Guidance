# ListInstance Class
 This class holds deprecated ListInstance properties and methods 

 Domain Object that specifies the properties of the new list.   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel](OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel.md)  
## Syntax
```C#
public class ListInstance: BaseModel, IEquatable<ListInstance>
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [ListInstance()](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.ctor1.md) | Constructor for ListInstance class 
| [ListInstance(IEnumerable<ContentTypeBinding>, IEnumerable<View>, IEnumerable<Field>, IEnumerable<FieldRef>, List<DataRow>)](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.ctor2.md) | Constructor for ListInstance class 
| [ListInstance(IEnumerable<ContentTypeBinding>, IEnumerable<View>, IEnumerable<Field>, IEnumerable<FieldRef>, List<DataRow>, Dictionary<String, String>, ObjectSecurity)](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.ctor3.md) | Constructor for ListInstance class 
| [ListInstance(IEnumerable<ContentTypeBinding>, IEnumerable<View>, IEnumerable<Field>, IEnumerable<FieldRef>, List<DataRow>, Dictionary<String, String>, ObjectSecurity, List<Folder>)](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.ctor4.md) | Constructor for ListInstance class 
| [ListInstance(IEnumerable<ContentTypeBinding>, IEnumerable<View>, IEnumerable<Field>, IEnumerable<FieldRef>, List<DataRow>, Dictionary<String, String>, ObjectSecurity, List<Folder>, List<CustomAction>)](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.ctor5.md) | Constructor for the ListInstance class 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [ContentTypeBindings](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.ContentTypeBindings.md) | Gets or sets the content types to associate to the list
| [ContentTypesEnabled](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.ContentTypesEnabled.md) | Gets or sets whether content types are enabled
| [DataRows](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.DataRows.md) | Gets or sets the DataRows associated to the list
| [DefaultDisplayFormUrl](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.DefaultDisplayFormUrl.md) | Defines a value that specifies the location of the default display form for the list.
| [DefaultEditFormUrl](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.DefaultEditFormUrl.md) | Defines a value that specifies the URL of the edit form to use for list items in the list.
| [DefaultNewFormUrl](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.DefaultNewFormUrl.md) | Defines a value that specifies the location of the default new form for the list.
| [Description](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.Description.md) | Gets or sets the description of the list
| [Direction](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.Direction.md) | Defines a value that specifies the reading order of the list.
| [DocumentTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.DocumentTemplate.md) | Gets or sets a value that specifies the identifier of the document template for the new list.
| [DraftVersionVisibility](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.DraftVersionVisibility.md) | Gets or sets the DraftVersionVisibility for the list
| [EnableAttachments](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.EnableAttachments.md) | Gets or sets whether attachments are enabled. Defaults to true.
| [EnableFolderCreation](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.EnableFolderCreation.md) | Gets or sets whether folder is enabled. Defaults to true.
| [EnableMinorVersions](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.EnableMinorVersions.md) | Gets or sets whether minor verisioning is enabled on the list
| [EnableModeration](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.EnableModeration.md) | Gets or sets whether moderation/content approval is enabled on the list
| [EnableVersioning](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.EnableVersioning.md) | Gets or sets whether verisioning is enabled on the list
| [FieldDefaults](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.FieldDefaults.md) | Defines a list of default values for the Fields of the List Instance
| [FieldRefs](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.FieldRefs.md) | Gets or sets the FieldRefs associated to the list
| [Fields](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.Fields.md) | Gets or sets the Fields associated to the list
| [Folders](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.Folders.md) | Defines a collection of folders (eventually nested) that will be provisioned into the target list/library
| [ForceCheckout](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.ForceCheckout.md) | Gets or sets whether to force checkout of documents in the library
| [Hidden](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.Hidden.md) | Gets or sets whether to hide the list
| [ImageUrl](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.ImageUrl.md) | Defines a value that specifies the URI for the icon of the list, optional attribute.
| [IrmExpire](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.IrmExpire.md) | Defines if IRM Expire property, optional attribute.
| [IrmReject](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.IrmReject.md) | Defines the IRM Reject property, optional attribute.
| [IRMSettings](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.IRMSettings.md) | 
| [IsApplicationList](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.IsApplicationList.md) | Defines a value that specifies a flag that a client application can use to determine whether to display the list, optional attribute.
| [ListExperience](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.ListExperience.md) | Defines the current list UI/UX experience (valid for SPO only).
| [MaxVersionLimit](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.MaxVersionLimit.md) | Gets or sets the MinorVersionLimit for verisioning, just in case it is enabled on the list
| [MinorVersionLimit](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.MinorVersionLimit.md) | Gets or sets the MinorVersionLimit for versioning, just in case it is enabled on the list
| [NoCrawl](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.NoCrawl.md) | Defines if the current list or library has to be included in crawling, optional attribute.
| [OnQuickLaunch](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.OnQuickLaunch.md) | Gets or sets a value that specifies whether the new list is displayed on the Quick Launch of the site.
| [ReadSecurity](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.ReadSecurity.md) | Defines the Read Security property, optional attribute.
| [RemoveExistingContentTypes](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.RemoveExistingContentTypes.md) | Gets or sets whether existing content types should be removed
| [RemoveExistingViews](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.RemoveExistingViews.md) | Gets or sets whether existing views should be removed
| [Security](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.Security.md) | Defines the Security rules for the List Instance
| [TemplateFeatureID](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.TemplateFeatureID.md) | Gets or sets the Guid for TemplateFeature
| [TemplateType](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.TemplateType.md) | Gets or sets a value that specifies the list server template of the new list. https://msdn.microsoft.com/en-us/library/office/microsoft.sharepoint.client.listtemplatetype.aspx
| [Title](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.Title.md) | Gets or sets the list title
| [Url](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.Url.md) | Gets or sets a value that specifies whether the new list is displayed on the Quick Launch of the site.
| [UserCustomActions](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.UserCustomActions.md) | Defines a collection of user custom actions that will be provisioned into the target list/library
| [ValidationFormula](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.ValidationFormula.md) | Defines a value that specifies the data validation criteria for a list item, optional attribute.
| [ValidationMessage](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.ValidationMessage.md) | Defines a value that specifies the error message returned when data validation fails for a list item, optional attribute.
| [Views](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.Views.md) | Gets or sets the views associated to the list
| [Webhooks](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.Webhooks.md) | 
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Equals(Object)](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.3520ddbb.md) | Compares object with ListInstance
| [Equals(ListInstance)](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.f4a95136.md) | Compares ListInstance object based on ContentTypesEnabled, Description, DocumentTemplate, EnableVersioning, EnableMinorVersions, EnableModeration, Hidden, MaxVersionLimit, MinorVersionLimit, OnQuickLaunch, EnableAttachments, EnableFolderCreation, ForceCheckOut, RemoveExistingContentTypes, TemplateType, Title, Url, TemplateFeatureID, RemoveExistingViews, ContentTypeBindings, View, Fields, FieldRefs, FieldDefaults, Security, Folders, UserCustomActions, Webhooks, IRMSettings, DefaultDisplayFormUrl, DefaultEditFormUrl, DefaultNewFormUrl, Direction, ImageUrl, IrmExpire, IrmReject, IsApplicationList, ReadSecurity, ValidationFormula, and ValidationMessage properties.
| [GetHashCode()](OfficeDevPnP.Core.Framework.Provisioning.Model.ListInstance.1c6872bd.md) | Gets the hash code
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
