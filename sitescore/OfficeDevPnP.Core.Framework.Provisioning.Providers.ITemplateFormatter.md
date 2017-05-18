# ITemplateFormatter Interface  
 Interface for basic capabilites that any Template Formatter should provide/support   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public interface ITemplateFormatter
```
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Initialize(TemplateProviderBase)](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateFormatter.d92f5067.md) | Method to initialize the formatter with the proper TemplateProvider instance
| [IsValid(Stream)](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateFormatter.13870f06.md) | Method to validate the content of a formatted template instace
| [ToFormattedTemplate(ProvisioningTemplate)](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateFormatter.34498a5d.md) | Method to format a ProvisioningTemplate into a formatted template
| [ToProvisioningTemplate(Stream)](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateFormatter.d70e8f84.md) | Method to convert a formatted template into a ProvisioningTemplate
| [ToProvisioningTemplate(Stream, String)](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateFormatter.fef913ef.md) | Method to convert a formatted template into a ProvisioningTemplate, based on a specific ID
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md)
