# ExtensibilityManager.ExecuteExtensibilityExtractionCallOut Method  
 Method to Invoke Custom Extraction Handlers.   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public ProvisioningTemplate ExecuteExtensibilityExtractionCallOut(ClientContext ctx, ExtensibilityHandler handler, ProvisioningTemplate template, ProvisioningTemplateCreationInformation creationInformation, PnPMonitoredScope scope)
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

  

#### creationInformation  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateCreationInformation](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateCreationInformation.md)  
&emsp;&emsp;The Provisioning Template creation information object  

  

#### scope  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Diagnostics.PnPMonitoredScope](OfficeDevPnP.Core.Diagnostics.PnPMonitoredScope.md)  
&emsp;&emsp;The PnPMonitoredScope of the current step in the pipeline  

  

### Return Value
Type: [ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  

## Remarks
 Ensure the ClientContext is not disposed in the custom provider. 
  
## See also
- [ExtensibilityManager](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.ExtensibilityManager.md) 
- [OfficeDevPnP.Core.Framework.Provisioning.Extensibility.ExtensiblityPipelineException](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.ExtensiblityPipelineException.md)
- System.ArgumentException
- System.ArgumentNullException
- [OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md) 
