# ITemplateProviderExtension Interface  
 Interface for extending the XMLTemplateProvider while retrieving a template   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public interface ITemplateProviderExtension
```
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [SupportsGetTemplatePostProcessing](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateProviderExtension.SupportsGetTemplatePostProcessing.md) | Declares whether the object supports post-processing during GetTemplate
| [SupportsGetTemplatePreProcessing](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateProviderExtension.SupportsGetTemplatePreProcessing.md) | Declares whether the object supports pre-processing during GetTemplate
| [SupportsSaveTemplatePostProcessing](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateProviderExtension.SupportsSaveTemplatePostProcessing.md) | Declares whether the object supports post-processing during SaveTemplate
| [SupportsSaveTemplatePreProcessing](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateProviderExtension.SupportsSaveTemplatePreProcessing.md) | Declares whether the object supports pre-processing during SaveTemplate
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Initialize(Object)](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateProviderExtension.f2c09c75.md) | Initialization method to setup the extension object
| [PostProcessGetTemplate(ProvisioningTemplate)](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateProviderExtension.49b25d63.md) | Method invoked after deserializing the template from the source repository
| [PostProcessSaveTemplate(Stream)](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateProviderExtension.6ade08bb.md) | Method invoked after serializing the template and before it is saved onto the target repository
| [PreProcessGetTemplate(Stream)](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateProviderExtension.395db8ff.md) | Method invoked before deserializing the template from the source repository
| [PreProcessSaveTemplate(ProvisioningTemplate)](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateProviderExtension.8485277f.md) | Method invoked before serializing the template and before it is saved onto the target repository
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md)
