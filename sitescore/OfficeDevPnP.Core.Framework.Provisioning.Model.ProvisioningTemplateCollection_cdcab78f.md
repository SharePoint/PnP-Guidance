# ProvisioningTemplateCollection&lt;T&gt; Class
 Generic collection of items stored in the ProvisioningTemplate graph   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;T  
## Syntax
```C#
public abstract class ProvisioningTemplateCollection<T>: Collection<T>, IProvisioningTemplateDescendant where T : BaseModel
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [ProvisioningTemplateCollection(ProvisioningTemplate)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection_cdcab78f.ctor1.md) | Custom constructor to manage the ParentTemplate for the collection and all the children of the collection 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [ParentTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection_cdcab78f.ParentTemplate.md) | References the parent ProvisioningTemplate for the current provisioning artifact
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [AddRange(IEnumerable&lt;T&gt;)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection_cdcab78f.c9396447.md) | Adds item to the collection
| [Find(Predicate&lt;T&gt;)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection_cdcab78f.a3f4e88c.md) | Finds an item matching a search predicate
| [FindIndex(Predicate&lt;T&gt;)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection_cdcab78f.da089b2f.md) | Finds index of the item matching the search predicate
| [FindIndex(Int32, Predicate&lt;T&gt;)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection_cdcab78f.a0b9537a.md) | Finds index of the item matching the search predicate based on start index provided.
| [FindIndex(Int32, Int32, Predicate&lt;T&gt;)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection_cdcab78f.d0beeaa1.md) | Finds index of the item matching the search predicate based on start index and count.
| [RemoveAll(Predicate&lt;T&gt;)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection_cdcab78f.519f9e70.md) | Removes all the matching indexes
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
