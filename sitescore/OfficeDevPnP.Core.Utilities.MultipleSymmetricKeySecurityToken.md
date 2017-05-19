# MultipleSymmetricKeySecurityToken Class
 Represents a security token which contains multiple security keys that are generated using symmetric algorithms.   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;System.IdentityModel.Tokens.SecurityToken  
## Syntax
```C#
public class MultipleSymmetricKeySecurityToken: SecurityToken
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [MultipleSymmetricKeySecurityToken(IEnumerable<Byte[]>)](OfficeDevPnP.Core.Utilities.MultipleSymmetricKeySecurityToken.ctor1.md) | Initializes a new instance of the MultipleSymmetricKeySecurityToken class. 
| [MultipleSymmetricKeySecurityToken(String, IEnumerable<Byte[]>)](OfficeDevPnP.Core.Utilities.MultipleSymmetricKeySecurityToken.ctor2.md) | Initializes a new instance of the MultipleSymmetricKeySecurityToken class. 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [Id](OfficeDevPnP.Core.Utilities.MultipleSymmetricKeySecurityToken.Id.md) | Gets the unique identifier of the security token.
| [SecurityKeys](OfficeDevPnP.Core.Utilities.MultipleSymmetricKeySecurityToken.SecurityKeys.md) | Gets the cryptographic keys associated with the security token.
| [ValidFrom](OfficeDevPnP.Core.Utilities.MultipleSymmetricKeySecurityToken.ValidFrom.md) | Gets the first instant in time at which this security token is valid.
| [ValidTo](OfficeDevPnP.Core.Utilities.MultipleSymmetricKeySecurityToken.ValidTo.md) | Gets the last instant in time at which this security token is valid.
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [MatchesKeyIdentifierClause(SecurityKeyIdentifierClause)](OfficeDevPnP.Core.Utilities.MultipleSymmetricKeySecurityToken.e7dce578.md) | Returns a value that indicates whether the key identifier for this instance can be resolved to the specified key identifier.
## See also
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)
