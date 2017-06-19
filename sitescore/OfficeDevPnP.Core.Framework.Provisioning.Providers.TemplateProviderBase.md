# TemplateProviderBase Class
 Handles methods for Template Provider   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase  
&emsp;[OfficeDevPnP.Core.Framework.Provisioning.Providers.Json.JsonTemplateProvider](OfficeDevPnP.Core.Framework.Provisioning.Providers.Json.JsonTemplateProvider.md)  
&emsp;[OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.XMLTemplateProvider](OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.XMLTemplateProvider.md)  
## Syntax
```C#
public abstract class TemplateProviderBase
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [TemplateProviderBase()](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.ctor1.md) | Default Constructor 
| [TemplateProviderBase(FileConnectorBase)](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.ctor2.md) | Constructor 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [Connector](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.Connector.md) | File Connector
| [Parameters](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.Parameters.md) | Template parameters
| [SupportsDelete](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.SupportsDelete.md) | Supports template delete
| [SupportsSave](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.SupportsSave.md) | Supports template save
| [Uri](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.Uri.md) | Uri of site
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Delete(String)](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.cf3d39fd.md) | Deletes ProvisioningTemplate
| [GetTemplate(String)](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.63314bcb.md) | Gets ProvisioningTemplate
| [GetTemplate(String, ITemplateProviderExtension[])](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.87e64e45.md) | Gets ProvisioningTemplate
| [GetTemplate(String, String)](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.787ac00e.md) | Gets ProvisioningTemplate
| [GetTemplate(String, ITemplateFormatter)](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.5ab3afb3.md) | Gets ProvisioningTemplate
| [GetTemplate(String, String, ITemplateFormatter)](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.250dcb85.md) | Gets ProvisioningTemplate
| [GetTemplate(String, String, ITemplateFormatter, ITemplateProviderExtension[])](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.cc9b66fa.md) | Gets ProvisioningTemplate
| [GetTemplates()](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.637e3e6b.md) | Gets list of ProvisioningTemplates
| [GetTemplates(ITemplateFormatter)](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.57d85359.md) | Gets list of ProvisioningTemplates
| [Save(ProvisioningTemplate)](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.da61c130.md) | Saves ProvisioningTemplate
| [Save(ProvisioningTemplate, ITemplateProviderExtension[])](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.1c9d227e.md) | Saves ProvisioningTemplate
| [Save(ProvisioningTemplate, ITemplateFormatter)](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.36e39e3.md) | Saves ProvisioningTemplate
| [Save(ProvisioningTemplate, ITemplateFormatter, ITemplateProviderExtension[])](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.575209b6.md) | Saves ProvisioningTemplate
| [SaveAs(ProvisioningTemplate, String)](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.c088c3c5.md) | Saves ProvisioningTemplate
| [SaveAs(ProvisioningTemplate, String, ITemplateProviderExtension[])](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.3b2e8cc2.md) | Saves ProvisioningTemplate
| [SaveAs(ProvisioningTemplate, String, ITemplateFormatter)](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.3ae34207.md) | Saves ProvisioningTemplate
| [SaveAs(ProvisioningTemplate, String, ITemplateFormatter, ITemplateProviderExtension[])](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.c9910f96.md) | Saves ProvisioningTemplate
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md)
