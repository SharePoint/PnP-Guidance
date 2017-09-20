# SharePointConnector Class
 Connector for files in SharePoint   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Connectors](OfficeDevPnP.Core.Framework.Provisioning.Connectors.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.md)  
## Syntax
```C#
public class SharePointConnector: FileConnectorBase
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [SharePointConnector()](OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector.ctor1.md) | Base constructor 
| [SharePointConnector(ClientRuntimeContext, String, String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector.ctor2.md) | SharePointConnector constructor. Allows to directly set root folder and sub folder 
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [DeleteFile(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector.9ad8acaf.md) | Deletes a file from the default container
| [DeleteFile(String, String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector.476dd1f3.md) | Deletes a file from the specified container
| [GetFile(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector.df261957.md) | Gets a file as string from the default container
| [GetFile(String, String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector.7ad54aac.md) | Gets a file as string from the specified container
| [GetFilenamePart(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector.9e3b826.md) | Returns a filename without a path
| [GetFiles()](OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector.1ef203bb.md) | Get the files available in the default container
| [GetFiles(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector.349a20d0.md) | Get the files available in the specified container
| [GetFileStream(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector.667e64b2.md) | Gets a file as stream from the default container
| [GetFileStream(String, String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector.e43bb5.md) | Gets a file as stream from the specified container
| [GetFolders()](OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector.183fc5f5.md) | Get the folders of the default container
| [GetFolders(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector.c388caf.md) | Get the folders of a specified container
| [SaveFileStream(String, Stream)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector.3b54d26b.md) | Saves a stream to the default container with the given name. If the file exists it will be overwritten
| [SaveFileStream(String, String, Stream)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.SharePointConnector.ec95a2c1.md) | Saves a stream to the specified container with the given name. If the file exists it will be overwritten
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Connectors](OfficeDevPnP.Core.Framework.Provisioning.Connectors.md)
