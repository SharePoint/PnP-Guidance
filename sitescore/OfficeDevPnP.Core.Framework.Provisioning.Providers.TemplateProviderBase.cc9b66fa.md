# TemplateProviderBase.GetTemplate Method  
 Gets ProvisioningTemplate   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public abstract ProvisioningTemplate GetTemplate(String uri, String identifier, ITemplateFormatter formatter, ITemplateProviderExtension[] extensions)
```
### Parameters
#### uri  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;A SharePoint uri  

  

#### identifier  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;ProvisioningTemplate identifier  

  

#### formatter  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateFormatter](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateFormatter.md)  
&emsp;&emsp;Provisioning Template formatter  

  

#### extensions  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateProviderExtension[]](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateProviderExtension.md)  
&emsp;&emsp;Collection of provisioning template extensions  

  

### Return Value
Type: [ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
Returns a ProvisioningTemplate  


## See also
- [TemplateProviderBase](OfficeDevPnP.Core.Framework.Provisioning.Providers.TemplateProviderBase.md) 
- [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md) 
