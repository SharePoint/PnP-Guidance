# IProvisioningExtensibilityHandler.Provision Method  
 Execute custom actions during provisioning of a template   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public abstract void Provision(ClientContext ctx, ProvisioningTemplate template, ProvisioningTemplateApplyingInformation applyingInformation, TokenParser tokenParser, PnPMonitoredScope scope, String configurationData)
```
### Parameters
#### ctx  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ClientContext  
&emsp;&emsp;The target ClientContext  

  

#### template  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
&emsp;&emsp;The current Provisioning Template  

  

#### applyingInformation  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateApplyingInformation](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateApplyingInformation.md)  
&emsp;&emsp;The Provisioning Template application information object  

  

#### tokenParser  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.TokenParser](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.TokenParser.md)  
&emsp;&emsp;Token parser instance  

  

#### scope  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Diagnostics.PnPMonitoredScope](OfficeDevPnP.Core.Diagnostics.PnPMonitoredScope.md)  
&emsp;&emsp;The PnPMonitoredScope of the current step in the pipeline  

  

#### configurationData  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The configuration data, if any, for the handler  

  

### Return Value
Type: void  

## See also
- [IProvisioningExtensibilityHandler](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.IProvisioningExtensibilityHandler.md) 
- [OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md) 
