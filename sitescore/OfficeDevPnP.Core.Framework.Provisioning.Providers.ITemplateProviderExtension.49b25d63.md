# ITemplateProviderExtension.PostProcessGetTemplate Method  
 Method invoked after deserializing the template from the source repository   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public abstract ProvisioningTemplate PostProcessGetTemplate(ProvisioningTemplate template)
```
### Parameters
#### template  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
&emsp;&emsp;The just deserialized template  

  

### Return Value
Type: [ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
The resulting template, after post-processing  


## See also
- [ITemplateProviderExtension](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateProviderExtension.md) 
- [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md) 
