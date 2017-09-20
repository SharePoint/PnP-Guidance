# IProvisioningExtensibilityHandler.Extract Method  
 Execute custom actions during extraction of a template   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public abstract ProvisioningTemplate Extract(ClientContext ctx, ProvisioningTemplate template, ProvisioningTemplateCreationInformation creationInformation, PnPMonitoredScope scope, String configurationData)
```
### Parameters
#### ctx  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ClientContext  
&emsp;&emsp;The target ClientContext  

  

#### template  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
&emsp;&emsp;The current Provisioning Template  

  

#### creationInformation  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateCreationInformation](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateCreationInformation.md)  
&emsp;&emsp;The Provisioning Template creation information object  

  

#### scope  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Diagnostics.PnPMonitoredScope](OfficeDevPnP.Core.Diagnostics.PnPMonitoredScope.md)  
&emsp;&emsp;The PnPMonitoredScope of the current step in the pipeline  

  

#### configurationData  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The configuration data, if any, for the handler  

  

### Return Value
Type: [ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
The Provisioning Template eventually enriched by the handler during extraction  


## See also
- [IProvisioningExtensibilityHandler](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.IProvisioningExtensibilityHandler.md) 
- [OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md) 
