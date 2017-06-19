# IProvisioningExtensibilityProvider.ProcessRequest Method  
 Defines a interface that accepts requests from the provisioning processing component   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public abstract void ProcessRequest(ClientContext ctx, ProvisioningTemplate template, String configurationData)
```
### Parameters
#### ctx  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ClientContext  
&emsp;&emsp;The ClientContext to process  

  

#### template  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
&emsp;&emsp;The Provisioning template  

  

#### configurationData  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Configuration Data string  

  

### Return Value
Type: void  

## See also
- [IProvisioningExtensibilityProvider](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.IProvisioningExtensibilityProvider.md) 
- [OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md) 
