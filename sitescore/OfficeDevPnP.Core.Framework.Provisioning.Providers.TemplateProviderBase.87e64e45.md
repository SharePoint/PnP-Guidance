# TemplateProviderBase.GetTemplate Method  
 Gets ProvisioningTemplate   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public abstract ProvisioningTemplate GetTemplate(String uri, ITemplateProviderExtension[] extensions)
```
### Parameters
#### uri  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;A SharePoint uri  

  

#### extensions  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateProviderExtension[]](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateProviderExtension.md)  
&emsp;&emsp;Collection of provisioning template extensions  

  

### Return Value
Type: [ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
Returns a ProvisioningTemplate  


## See also
- [TemplateProviderBase](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.md) 
- [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md) 
