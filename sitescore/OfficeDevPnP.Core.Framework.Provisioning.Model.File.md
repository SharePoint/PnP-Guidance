# File Class
 Defines a File element, to describe a file that will be provisioned into the target Site   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel](OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel.md)  
## Syntax
```C#
public class File: BaseModel, IEquatable<File>
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [File()](OfficeDevPnP.Core.Framework.Provisioning.Model.File.ctor1.md) | Constructor for the File class 
| [File(String, String, Boolean, IEnumerable<WebPart>, IDictionary<String, String>, ObjectSecurity, FileLevel)](OfficeDevPnP.Core.Framework.Provisioning.Model.File.ctor2.md) | Constructor for the File class 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [Folder](OfficeDevPnP.Core.Framework.Provisioning.Model.File.Folder.md) | The TargetFolder of the File
| [Level](OfficeDevPnP.Core.Framework.Provisioning.Model.File.Level.md) | The Level status for the File
| [Overwrite](OfficeDevPnP.Core.Framework.Provisioning.Model.File.Overwrite.md) | The Overwrite flag for the File
| [Properties](OfficeDevPnP.Core.Framework.Provisioning.Model.File.Properties.md) | Properties of the file
| [Security](OfficeDevPnP.Core.Framework.Provisioning.Model.File.Security.md) | Defines the Security rules for the File
| [Src](OfficeDevPnP.Core.Framework.Provisioning.Model.File.Src.md) | The Src of the File
| [TargetFileName](OfficeDevPnP.Core.Framework.Provisioning.Model.File.TargetFileName.md) | The Target file name for the File, optional attribute. If missing, the original file name will be used.
| [WebParts](OfficeDevPnP.Core.Framework.Provisioning.Model.File.WebParts.md) | Webparts in the file
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Equals(Object)](OfficeDevPnP.Core.Framework.Provisioning.Model.File.3520ddbb.md) | Compares object with File
| [Equals(File)](OfficeDevPnP.Core.Framework.Provisioning.Model.File.fd046a34.md) | Compares File object based on Folder, Overwrite, Src, WebParts, Properties, Security, and TargetFileName.
| [GetHashCode()](OfficeDevPnP.Core.Framework.Provisioning.Model.File.1c6872bd.md) | Gets the hash code
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
