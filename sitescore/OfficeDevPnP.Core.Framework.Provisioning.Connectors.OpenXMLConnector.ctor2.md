# OpenXMLConnector.OpenXMLConnector members 
 OpenXMLConnector constructor. Allows to manage a .PNP OpenXML package file through a supporting persistence connector.   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Connectors](OfficeDevPnP.Core.Framework.Provisioning.Connectors.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public OpenXMLConnector(string packageFileName, FileConnectorBase persistenceConnector, string author, X509Certificate2 signingCertificate)
```
### Parameters
#### packageFileName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The name of the .PNP package file. If the .PNP extension is missing, it will be added  


#### persistenceConnector  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.md)  
&emsp;&emsp;The FileConnector object that will be used for physical persistence of the file  


#### (optional) author  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The Author of the .PNP package file, if any. Optional  


#### (optional) signingCertificate  
&emsp;&emsp;Type: System.Security.Cryptography.X509Certificates.X509Certificate2  
&emsp;&emsp;The X.509 certificate to use for digital signature of the template, optional  


## See also
- [OpenXMLConnector](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXMLConnector.md)
- [OfficeDevPnP.Core.Framework.Provisioning.Connectors](OfficeDevPnP.Core.Framework.Provisioning.Connectors.md)
