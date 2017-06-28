# ProvisioningTemplateCollection&lt;T&gt;.Find Method  
 Finds an item matching a search predicate   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public T Find(Predicate<T> match)
```
### Parameters
#### match  
&emsp;&emsp;Type: System.Predicate&lt;T&gt;  
&emsp;&emsp;The matching predicate to use for finding any target item  

  

### Return Value
Type: T  
The target item matching the find predicate  


## Remarks
We implemented this to adhere to the generic List of T behavior
  
## See also
- [ProvisioningTemplateCollection&lt;T&gt;](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplateCollection_cdcab78f.md) 
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md) 
