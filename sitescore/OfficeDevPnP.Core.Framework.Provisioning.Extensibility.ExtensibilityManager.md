# ExtensibilityManager Class
 Provisioning Framework Component that is used for invoking custom providers during the provisioning process. 

 Provisioning Framework Component that is used for invoking custom providers during the provisioning process.   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public class ExtensibilityManager
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [ExtensibilityManager()](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.ExtensibilityManager.ctor1.md) |  Provisioning Framework Component that is used for invoking custom providers during the provisioning process. Provisioning Framework Component that is used for invoking custom providers during the provisioning process. 
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [ExecuteExtensibilityCallOut(ClientContext, ExtensibilityHandler, ProvisioningTemplate)](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.ExtensibilityManager.36a5e1b4.md) | Method to Invoke Custom Provisioning Providers. Ensure the ClientContext is not disposed in the custom provider.
| [ExecuteExtensibilityExtractionCallOut(ClientContext, ExtensibilityHandler, ProvisioningTemplate, ProvisioningTemplateCreationInformation, PnPMonitoredScope)](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.ExtensibilityManager.44bd95c4.md) | Method to Invoke Custom Extraction Handlers.
| [ExecuteExtensibilityProvisionCallOut(ClientContext, ExtensibilityHandler, ProvisioningTemplate, ProvisioningTemplateApplyingInformation, TokenParser, PnPMonitoredScope)](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.ExtensibilityManager.2db05b82.md) | Method to Invoke Custom Provisioning Handlers.
| [ExecuteTokenProviderCallOut(ClientContext, ExtensibilityHandler, ProvisioningTemplate)](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.ExtensibilityManager.2865f124.md) | Method to Invoke Custom Provisioning Token Providers which implement the IProvisioningExtensibilityTokenProvider interface. Ensure the ClientContext is not disposed in the custom provider.
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Extensibility.ExtensiblityPipelineException](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.ExtensiblityPipelineException.md)
- System.ArgumentException
- System.ArgumentNullException
- [OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md)
