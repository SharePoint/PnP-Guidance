# Folder Class
 Defines a folder that will be provisioned into the target list/library   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel](OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel.md)  
## Syntax
```C#
public class Folder: BaseModel, IEquatable<Folder>
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [Folder()](OfficeDevPnP.Core.Framework.Provisioning.Model.Folder.ctor1.md) | Constructor for the Folder class 
| [Folder(String, List<Folder>, ObjectSecurity)](OfficeDevPnP.Core.Framework.Provisioning.Model.Folder.ctor2.md) | Constructor for the Folder class 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [Folders](OfficeDevPnP.Core.Framework.Provisioning.Model.Folder.Folders.md) | Defines the child folders of the current Folder, if any
| [Name](OfficeDevPnP.Core.Framework.Provisioning.Model.Folder.Name.md) | The Name of the Folder
| [PropertyBagEntries](OfficeDevPnP.Core.Framework.Provisioning.Model.Folder.PropertyBagEntries.md) | 
| [Security](OfficeDevPnP.Core.Framework.Provisioning.Model.Folder.Security.md) | Defines the security rules for the current Folder
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Equals(Object)](OfficeDevPnP.Core.Framework.Provisioning.Model.Folder.3520ddbb.md) | Compares object with Folder
| [Equals(Folder)](OfficeDevPnP.Core.Framework.Provisioning.Model.Folder.4b857f24.md) | Compares Folder object based on Name, Folders and Security properties.
| [GetHashCode()](OfficeDevPnP.Core.Framework.Provisioning.Model.Folder.1c6872bd.md) | Gets the hash code
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
