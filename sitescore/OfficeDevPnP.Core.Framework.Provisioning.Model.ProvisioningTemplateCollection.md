# ProvisioningTemplateCollection Class
 Generic collection of items stored in the ProvisioningTemplate graph   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;T  
## Syntax
```C#
public abstract class ProvisioningTemplateCollectionT: Collection<T>, IProvisioningTemplateDescendant where T : BaseModel
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [ProvisioningTemplateCollection(ProvisioningTemplate)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection.ctor1.md) | Custom constructor to manage the ParentTemplate for the collection and all the children of the collection 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [ParentTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection.ParentTemplate.md) | References the parent ProvisioningTemplate for the current provisioning artifact
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [AddRange(IEnumerable&lt;T&gt;)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection.c9396447.md) | 
| [Find(Predicate&lt;T&gt;)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection.a3f4e88c.md) | Finds an item matching a search predicate
| [FindIndex(Predicate&lt;T&gt;)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection.da089b2f.md) | 
| [FindIndex(Int32, Predicate&lt;T&gt;)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection.a0b9537a.md) | 
| [FindIndex(Int32, Int32, Predicate&lt;T&gt;)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection.d0beeaa1.md) | 
| [RemoveAll(Predicate&lt;T&gt;)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection.519f9e70.md) | 
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
