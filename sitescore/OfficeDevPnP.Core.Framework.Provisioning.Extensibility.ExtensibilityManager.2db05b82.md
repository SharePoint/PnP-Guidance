# ExtensibilityManager.ExecuteExtensibilityProvisionCallOut Method  
 Method to Invoke Custom Provisioning Handlers.   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public void ExecuteExtensibilityProvisionCallOut(ClientContext ctx, ExtensibilityHandler handler, ProvisioningTemplate template, ProvisioningTemplateApplyingInformation applyingInformation, TokenParser tokenParser, PnPMonitoredScope scope)
```
### Parameters
#### ctx  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ClientContext  
&emsp;&emsp;Authenticated ClientContext that is passed to the custom provider.  

  

#### handler  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.Model.ExtensibilityHandler](OfficeDevPnP.Core.Framework.Provisioning.Model.ExtensibilityHandler.md)  
&emsp;&emsp;A custom Extensibility Provisioning Provider  

  

#### template  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
&emsp;&emsp;ProvisioningTemplate that is passed to the custom provider  

  

#### applyingInformation  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateApplyingInformation](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateApplyingInformation.md)  
&emsp;&emsp;The Provisioning Template application information object  

  

#### tokenParser  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.TokenParser](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.TokenParser.md)  
&emsp;&emsp;The Token Parser used by the engine during template provisioning  

  

#### scope  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Diagnostics.PnPMonitoredScope](OfficeDevPnP.Core.Diagnostics.PnPMonitoredScope.md)  
&emsp;&emsp;The PnPMonitoredScope of the current step in the pipeline  

  

### Return Value
Type: void  

## Remarks
 Ensure the ClientContext is not disposed in the custom provider. 
  
## See also
- [ExtensibilityManager](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.ExtensibilityManager.md) 
- [OfficeDevPnP.Core.Framework.Provisioning.Extensibility.ExtensiblityPipelineException](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.ExtensiblityPipelineException.md)
- System.ArgumentException
- System.ArgumentNullException
- [OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md) 
