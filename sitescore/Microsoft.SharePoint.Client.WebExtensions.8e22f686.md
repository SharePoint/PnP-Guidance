# WebExtensions.GetProvisioningTemplate Method  
 Can be used to extract custom provisioning template from existing site. The extracted template will be compared with the default base template.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static ProvisioningTemplate GetProvisioningTemplate(this Web web, ProvisioningTemplateCreationInformation creationInfo)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to get template from  

  

#### creationInfo  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateCreationInformation](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateCreationInformation.md)  
&emsp;&emsp;Specifies additional settings and/or properties  

  

### Return Value
Type: [ProvisioningTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.md)  
ProvisioningTemplate object with generated values from existing site  


## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
