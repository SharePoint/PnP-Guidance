# OpenXMLConnector Class
 Connector that stores all the files into a unique .PNP OpenXML package   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Connectors](OfficeDevPnP.Core.Framework.Provisioning.Connectors.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.md)  
## Syntax
```C#
public class OpenXMLConnector: FileConnectorBase, ICommitableFileConnector
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [OpenXMLConnector(Stream)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.ctor1.md) | OpenXMLConnector constructor. Allows to manage a .PNP OpenXML package through an in memory stream. 
| [OpenXMLConnector(String, FileConnectorBase, String, X509Certificate2)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.ctor2.md) | OpenXMLConnector constructor. Allows to manage a .PNP OpenXML package file through a supporting persistence connector. 
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Commit()](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.17c9d8e5.md) | Commits the file
| [DeleteFile(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.9ad8acaf.md) | Deletes a file from the default container
| [DeleteFile(String, String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.476dd1f3.md) | Deletes a file from the specified container
| [GetFile(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.df261957.md) | Gets a file as string from the default container
| [GetFile(String, String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.7ad54aac.md) | Gets a file as string from the specified container
| [GetFilenamePart(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.9e3b826.md) | Returns a filename without a path
| [GetFiles()](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.1ef203bb.md) | Get the files available in the default container
| [GetFiles(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.349a20d0.md) | Get the files available in the specified container
| [GetFileStream(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.667e64b2.md) | Gets a file as stream from the default container
| [GetFileStream(String, String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.e43bb5.md) | Gets a file as stream from the specified container
| [GetFolders()](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.183fc5f5.md) | Get the folders of the default container
| [GetFolders(String)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.c388caf.md) | Get the folders of a specified container
| [SaveFileStream(String, Stream)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.3b54d26b.md) | Saves a stream to the default container with the given name. If the file exists it will be overwritten
| [SaveFileStream(String, String, Stream)](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.ec95a2c1.md) | Saves a stream to the specified container with the given name. If the file exists it will be overwritten
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Connectors](OfficeDevPnP.Core.Framework.Provisioning.Connectors.md)
