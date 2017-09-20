# ProvisioningTemplateApplyingInformation Class
 Handles methods for applying provisioning templates   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public class ProvisioningTemplateApplyingInformation
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [ProvisioningTemplateApplyingInformation()](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateApplyingInformation.ctor1.md) |  Handles methods for applying provisioning templates 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [ClearNavigation](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateApplyingInformation.ClearNavigation.md) | If true, existing navigation nodes of the site (where applicable) will be cleared out before applying the navigation nodes from the template (if any). This setting will override any settings made in the template.
| [ExtensibilityHandlers](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateApplyingInformation.ExtensibilityHandlers.md) | List of ExtensibilityHandlers
| [HandlersToProcess](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateApplyingInformation.HandlersToProcess.md) | Lists of Handlers to process
| [IgnoreDuplicateDataRowErrors](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateApplyingInformation.IgnoreDuplicateDataRowErrors.md) | If true then duplicate id errors when the same importing datarows simply generate a warning don't stop the engine. Reason for this is being able to apply the same template multiple times (Delta handling) without that failing cause the same record is being added twice
| [MessagesDelegate](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateApplyingInformation.MessagesDelegate.md) | 
| [OverwriteSystemPropertyBagValues](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateApplyingInformation.OverwriteSystemPropertyBagValues.md) | If true, system propertybag entries that start with _, vti_, dlc_ etc. will be overwritten if overwrite = true on the PropertyBagEntry. If not true those keys will be skipped, regardless of the overwrite property of the entry.
| [PersistTemplateInfo](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateApplyingInformation.PersistTemplateInfo.md) | If true then persists template information
| [ProgressDelegate](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateApplyingInformation.ProgressDelegate.md) | 
| [ProvisionContentTypesToSubWebs](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.ProvisioningTemplateApplyingInformation.ProvisionContentTypesToSubWebs.md) | If true then any content types in the template will be provisioned to subwebs
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.md)
