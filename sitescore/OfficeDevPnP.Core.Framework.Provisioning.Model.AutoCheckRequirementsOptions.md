# AutoCheckRequirementsOptions  enumeration
Defines how an engine should behave if the requirements for provisioning publishing capabilities are not satisfied by the target site  

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public enum AutoCheckRequirementsOptions
```
## Members
|**Member Name**|**Description**|
|:-----|:-----|
| MakeCompliant | Instructs the engine to make the target site compliant with the requirements
| SkipIfNotCompliant | Instructs the engine to skip the Publishing section if the target site is not compliant with the requirements
| FailIfNotCompliant | Instructs the engine to throw an exception/failure if the target site is not compliant with the requirements

## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
