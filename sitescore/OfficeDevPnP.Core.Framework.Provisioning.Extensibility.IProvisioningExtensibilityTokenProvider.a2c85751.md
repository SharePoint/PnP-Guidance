# IProvisioningExtensibilityTokenProvider.GetTokens Method  
 Provides Token Definitions to the template provisioning pipeline   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public IEnumerable<TokenDefinition> GetTokens(ClientContext ctx, ProvisioningTemplate template, String configurationData)
```
### Parameters
#### ctx  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ClientContext  
&emsp;&emsp; Provides Token Definitions to the template provisioning pipeline   

  

#### template  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
&emsp;&emsp; Provides Token Definitions to the template provisioning pipeline   

  

#### configurationData  
&emsp;&emsp;Type: System.String  
&emsp;&emsp; Provides Token Definitions to the template provisioning pipeline   

  

### Return Value
Type: IEnumerable<TokenDefinition>  

## See also
- [IProvisioningExtensibilityTokenProvider](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.IProvisioningExtensibilityTokenProvider.md) 
- [OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md) 
