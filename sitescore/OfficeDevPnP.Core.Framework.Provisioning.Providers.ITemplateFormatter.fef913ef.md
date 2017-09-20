# ITemplateFormatter.ToProvisioningTemplate Method  
 Method to convert a formatted template into a ProvisioningTemplate, based on a specific ID   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public abstract ProvisioningTemplate ToProvisioningTemplate(Stream template, String identifier)
```
### Parameters
#### template  
&emsp;&emsp;Type: System.IO.Stream  
&emsp;&emsp;The input formatted template as a Stream  

  

#### identifier  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The identifier of the template to convert  

  

### Return Value
Type: [ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
The output ProvisioningTemplate  


## See also
- [ITemplateFormatter](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateFormatter.md) 
- [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md) 
