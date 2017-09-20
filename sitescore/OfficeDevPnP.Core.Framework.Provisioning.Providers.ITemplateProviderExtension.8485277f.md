# ITemplateProviderExtension.PreProcessSaveTemplate Method  
 Method invoked before serializing the template and before it is saved onto the target repository   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public abstract ProvisioningTemplate PreProcessSaveTemplate(ProvisioningTemplate template)
```
### Parameters
#### template  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
&emsp;&emsp;The template that is going to be serialized  

  

### Return Value
Type: [ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
The resulting template, after pre-processing  


## See also
- [ITemplateProviderExtension](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateProviderExtension.md) 
- [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md) 
