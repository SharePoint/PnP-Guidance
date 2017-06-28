# BaseTemplateManager.GetBaseTemplate Method  
 Gets the provisioning template of provided webtemplate and configuration.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static ProvisioningTemplate GetBaseTemplate(this Web web, String webTemplate, Int16 configuration)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;the target web  

  

#### webTemplate  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;the name of the webtemplate  

  

#### configuration  
&emsp;&emsp;Type: System.Int16  
&emsp;&emsp;configuration of template  

  

### Return Value
Type: [ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
Returns a ProvisioningTemplate object  


## See also
- [BaseTemplateManager](Microsoft.SharePoint.Client.BaseTemplateManager.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
