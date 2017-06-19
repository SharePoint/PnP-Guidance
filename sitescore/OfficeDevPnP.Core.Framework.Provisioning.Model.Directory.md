# Directory Class
 Defines a Directory element, to describe a folder in the current repository that will be used to upload files into the target Site   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel](OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel.md)  
## Syntax
```C#
public class Directory: BaseModel, IEquatable<Directory>
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [Directory()](OfficeDevPnP.Core.Framework.Provisioning.Model.Directory.ctor1.md) | Constructor for Directory class 
| [Directory(String, String, Boolean, FileLevel, Boolean, String, String, String, ObjectSecurity)](OfficeDevPnP.Core.Framework.Provisioning.Model.Directory.ctor2.md) | Constructor for Directory class 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [ExcludedExtensions](OfficeDevPnP.Core.Framework.Provisioning.Model.Directory.ExcludedExtensions.md) | The file Extensions to exclude while uploading the Directory
| [Folder](OfficeDevPnP.Core.Framework.Provisioning.Model.Directory.Folder.md) | The TargetFolder of the Directory
| [IncludedExtensions](OfficeDevPnP.Core.Framework.Provisioning.Model.Directory.IncludedExtensions.md) | The file Extensions to include while uploading the Directory
| [Level](OfficeDevPnP.Core.Framework.Provisioning.Model.Directory.Level.md) | The Level status for the files in the Directory
| [MetadataMappingFile](OfficeDevPnP.Core.Framework.Provisioning.Model.Directory.MetadataMappingFile.md) | The file path of JSON mapping file with metadata for files to upload in the Directory
| [Overwrite](OfficeDevPnP.Core.Framework.Provisioning.Model.Directory.Overwrite.md) | The Overwrite flag for the files in the Directory
| [Recursive](OfficeDevPnP.Core.Framework.Provisioning.Model.Directory.Recursive.md) | Defines whether to recursively browse through all the child folders of the Directory
| [Security](OfficeDevPnP.Core.Framework.Provisioning.Model.Directory.Security.md) | Defines the Security rules for the File
| [Src](OfficeDevPnP.Core.Framework.Provisioning.Model.Directory.Src.md) | The Src of the Directory
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Equals(Object)](OfficeDevPnP.Core.Framework.Provisioning.Model.Directory.3520ddbb.md) | Compares object with Directory
| [Equals(Directory)](OfficeDevPnP.Core.Framework.Provisioning.Model.Directory.dbc03230.md) | Compares Directory object based on ExcludedExtensions, Folder, IncludedExtensions, Level, MetaDataMappingFile, Overwrite, Recursive, Src and Security properties.
| [GetHashCode()](OfficeDevPnP.Core.Framework.Provisioning.Model.Directory.1c6872bd.md) | Gets the hash code
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
