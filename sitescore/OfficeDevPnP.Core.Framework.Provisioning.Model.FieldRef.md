# FieldRef Class
 Represents a Field XML Markup that is used to define information about a field 

 Represents a Field XML Markup that is used to define information about a field   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel](OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel.md)  
## Syntax
```C#
public class FieldRef: BaseModel, IEquatable<FieldRef>
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [FieldRef()](OfficeDevPnP.Core.Framework.Provisioning.Model.FieldRef.ctor1.md) | Constructor for FieldRef class 
| [FieldRef(String)](OfficeDevPnP.Core.Framework.Provisioning.Model.FieldRef.ctor2.md) | Constructor for FieldRef class 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [DisplayName](OfficeDevPnP.Core.Framework.Provisioning.Model.FieldRef.DisplayName.md) | Gets or sets the Display Name of the field. Only applicable to fields associated with lists.
| [Hidden](OfficeDevPnP.Core.Framework.Provisioning.Model.FieldRef.Hidden.md) | Gets or sets if the field is Hidden
| [Id](OfficeDevPnP.Core.Framework.Provisioning.Model.FieldRef.Id.md) | Gets ot sets the ID of the referenced field
| [Name](OfficeDevPnP.Core.Framework.Provisioning.Model.FieldRef.Name.md) | Gets or sets the name of the field link. This will not change the internal name of the field.
| [Remove](OfficeDevPnP.Core.Framework.Provisioning.Model.FieldRef.Remove.md) | Declares if the FieldRef should be Removed from the list or library, optional attribute.
| [Required](OfficeDevPnP.Core.Framework.Provisioning.Model.FieldRef.Required.md) | Gets or sets if the field is Required
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Equals(Object)](OfficeDevPnP.Core.Framework.Provisioning.Model.FieldRef.3520ddbb.md) | Compares object with FieldRef
| [Equals(FieldRef)](OfficeDevPnP.Core.Framework.Provisioning.Model.FieldRef.492a3778.md) | Compares FieldRef object based on Id, Required, Hidden, and Remove properties.
| [GetHashCode()](OfficeDevPnP.Core.Framework.Provisioning.Model.FieldRef.1c6872bd.md) | Gets the hash code
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
