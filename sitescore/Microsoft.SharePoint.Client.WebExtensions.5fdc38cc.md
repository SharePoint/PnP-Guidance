# WebExtensions.ApplyProvisioningTemplate Method  
 Can be used to apply custom remote provisioning template on top of existing site.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void ApplyProvisioningTemplate(Web web, ProvisioningTemplate template, ProvisioningTemplateApplyingInformation applyingInformation)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp; Can be used to apply custom remote provisioning template on top of existing site.   

  

#### template  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
&emsp;&emsp;ProvisioningTemplate with the settings to be applied  

  

#### (optional) applyingInformation  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateApplyingInformation](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateApplyingInformation.md)  
&emsp;&emsp;Specified additional settings and or properties  

  

### Return Value
Type: void  

## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
