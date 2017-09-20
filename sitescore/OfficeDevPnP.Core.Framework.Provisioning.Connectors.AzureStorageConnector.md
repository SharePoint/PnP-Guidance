# AzureStorageConnector Class
 Connector for files in Azure blob storage   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Connectors](OfficeDevPnP.Core.Framework.Provisioning.Connectors.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.md)  
## Syntax
```C#
public class AzureStorageConnector: FileConnectorBase
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [AzureStorageConnector()](OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector.ctor1.md) | Base constructor 
| [AzureStorageConnector(String, String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector.ctor2.md) | AzureStorageConnector constructor. Allows to directly set Azure Storage key and container 
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [DeleteFile(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector.9ad8acaf.md) | Deletes a file from the default container
| [DeleteFile(String, String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector.476dd1f3.md) | Deletes a file from the specified container
| [GetFile(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector.df261957.md) | Gets a file as string from the default container
| [GetFile(String, String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector.7ad54aac.md) | Gets a file as string from the specified container
| [GetFilenamePart(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector.9e3b826.md) | Returns a filename without a path
| [GetFiles()](OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector.1ef203bb.md) | Get the files available in the default container
| [GetFiles(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector.349a20d0.md) | Get the files available in the specified container
| [GetFileStream(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector.667e64b2.md) | Gets a file as stream from the default container
| [GetFileStream(String, String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector.e43bb5.md) | Gets a file as stream from the specified container
| [GetFolders()](OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector.183fc5f5.md) | Get the folders of the default container
| [GetFolders(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector.c388caf.md) | Get the folders of a specified container
| [SaveFileStream(String, Stream)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector.3b54d26b.md) | Saves a stream to the default container with the given name. If the file exists it will be overwritten
| [SaveFileStream(String, String, Stream)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.AzureStorageConnector.ec95a2c1.md) | Saves a stream to the specified container with the given name. If the file exists it will be overwritten
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Connectors](OfficeDevPnP.Core.Framework.Provisioning.Connectors.md)
