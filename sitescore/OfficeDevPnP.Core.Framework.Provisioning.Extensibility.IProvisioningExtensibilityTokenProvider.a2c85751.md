# IProvisioningExtensibilityTokenProvider.GetTokens Method  
 Provides Token Definitions to the template provisioning pipeline   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public abstract IEnumerable<TokenDefinition> GetTokens(ClientContext ctx, ProvisioningTemplate template, String configurationData)
```
### Parameters
#### ctx  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ClientContext  
&emsp;&emsp;The ClientContext  

  

#### template  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
&emsp;&emsp;The Provisioning template  

  

#### configurationData  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Configuration Data string  

  

### Return Value
Type: IEnumerable<TokenDefinition>  

## See also
- [IProvisioningExtensibilityTokenProvider](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.IProvisioningExtensibilityTokenProvider.md) 
- [OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md) 
