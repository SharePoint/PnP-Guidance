# ProvisioningTemplateDictionary&lt;TKey, TItem&gt; Class
 Generic keyed collection of items stored in the ProvisioningTemplate graph   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;TKey,TItem  
## Syntax
```C#
public abstract class ProvisioningTemplateDictionary<TKey, TItem>: KeyedCollection<TKey, TItem>, IProvisioningTemplateDescendant where TItem : BaseModel
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [ProvisioningTemplateDictionary(ProvisioningTemplate)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateDictionary_cdcab78e.ctor1.md) | Custom constructor to manage the ParentTemplate for the collection and all the children of the collection 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [ParentTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateDictionary_cdcab78e.ParentTemplate.md) | References the parent ProvisioningTemplate for the current provisioning artifact
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
