# ContentType Class
 Domain Object used in the Provisioning template that defines a Content Type https://msdn.microsoft.com/en-us/library/office/ms463449.aspx  

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel](OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel.md)  
## Syntax
```C#
public class ContentType: BaseModel, IEquatable<ContentType>
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [ContentType()](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.ctor1.md) | Constructor for ContentType class 
| [ContentType(String, String, String, String, Boolean, Boolean, Boolean, String, Boolean, IEnumerable<FieldRef>)](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.ctor2.md) | Constructor for ContentType class 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [Description](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.Description.md) | The description of the Content Type
| [DisplayFormUrl](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.DisplayFormUrl.md) | Specifies the URL of a custom display form to use for list items that have been assigned the content type
| [DocumentSetTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.DocumentSetTemplate.md) | Specifies the properties of the DocumentSet Template if the ContentType defines a DocumentSet
| [DocumentTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.DocumentTemplate.md) | Specifies the document template for the content type
| [EditFormUrl](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.EditFormUrl.md) | Specifies the URL of a custom edit form to use for list items that have been assigned the content type
| [FieldRefs](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.FieldRefs.md) | The FieldRefs entries of the List Instance
| [Group](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.Group.md) | The group name of the content type
| [Hidden](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.Hidden.md) | True to define the content type as hidden. If you define a content type as hidden, SharePoint Foundation does not display that content type on the New button in list views.
| [Id](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.Id.md) | The Id of the Content Type
| [Name](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.Name.md) | The name of the Content Type
| [NewFormUrl](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.NewFormUrl.md) | Specifies the URL of a custom new form to use for list items that have been assigned the content type
| [Overwrite](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.Overwrite.md) | True to overwrite an existing content type with the same ID.
| [ReadOnly](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.ReadOnly.md) | True to specify that the content type cannot be edited without explicitly removing the read-only setting. This can be done either in the user interface or in code.
| [Sealed](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.Sealed.md) | True to prevent changes to this content type. You cannot change the value of this attribute through the user interface, but you can change it in code if you have sufficient rights. You must have site collection administrator rights to unseal a content type.
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Equals(Object)](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.3520ddbb.md) | Compares object with ContentType
| [Equals(ContentType)](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.f2a50643.md) | Compares ContentType object based on Id, Name, Description, Group, Hidden, RedOnly, Overwrite, Sealed, DocumentTemplate, DocumentSetTemplate and FieldRefs properties.
| [GetHashCode()](OfficeDevPnP.Core.Framework.Provisioning.Model.ContentType.1c6872bd.md) | Gets the hash code
## See also
- [https://msdn.microsoft.com/en-us/library/office/ms463449.aspx](https://msdn.microsoft.com/en-us/library/office/ms463449.aspx)
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
