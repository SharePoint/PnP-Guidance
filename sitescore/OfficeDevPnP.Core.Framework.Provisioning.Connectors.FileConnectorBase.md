# FileConnectorBase Class
 Base file connector class   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Connectors](OfficeDevPnP.Core.Framework.Provisioning.Connectors.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase  
&emsp;[OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector](OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector.md)  
&emsp;[OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileSystemConnector](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileSystemConnector.md)  
&emsp;[OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.md)  
&emsp;[OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector](OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector.md)  
## Syntax
```C#
public abstract class FileConnectorBase
```
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [Parameters](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.Parameters.md) | Parameters required for the file.
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [AddParameter(String, Object)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.5427f8bb.md) | Adds Parameter as an object.
| [AddParameterAsString(String, String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.3a5ffa18.md) | Adds Parameter as a string.
| [DeleteFile(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.9ad8acaf.md) | Deletes a file from the default container
| [DeleteFile(String, String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.476dd1f3.md) | Deletes a file from the specified container
| [GetFile(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.df261957.md) | Gets a file as string from the default container
| [GetFile(String, String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.7ad54aac.md) | Gets a file as string from the specified container
| [GetFilenamePart(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.9e3b826.md) | Returns a filename without a path
| [GetFiles()](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.1ef203bb.md) | Get the files available in the default container
| [GetFiles(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.349a20d0.md) | Get the files available in the specified container
| [GetFileStream(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.667e64b2.md) | Gets a file as stream from the default container
| [GetFileStream(String, String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.e43bb5.md) | Gets a file as stream from the specified container
| [GetFolders()](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.183fc5f5.md) | Get the folders of the default container
| [GetFolders(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.c388caf.md) | Get the folders of a specified container
| [SaveFileStream(String, Stream)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.3b54d26b.md) | Saves a stream to the default container with the given name. If the file exists it will be overwritten
| [SaveFileStream(String, String, Stream)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.ec95a2c1.md) | Saves a stream to the specified container with the given name. If the file exists it will be overwritten
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Connectors](OfficeDevPnP.Core.Framework.Provisioning.Connectors.md)
