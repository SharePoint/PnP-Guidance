# MultipleSymmetricKeySecurityToken.MatchesKeyIdentifierClause Method  
 Returns a value that indicates whether the key identifier for this instance can be resolved to the specified key identifier.   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public override bool MatchesKeyIdentifierClause(SecurityKeyIdentifierClause keyIdentifierClause)
```
### Parameters
#### keyIdentifierClause  
&emsp;&emsp;Type: System.IdentityModel.Tokens.SecurityKeyIdentifierClause  
&emsp;&emsp;A SecurityKeyIdentifierClause to compare to this instance  

  

### Return Value
Type: bool  
true if keyIdentifierClause is a SecurityKeyIdentifierClause and it has the same unique identifier as the Id property; otherwise, false.  


## See also
- [MultipleSymmetricKeySecurityToken](OfficeDevPnP.Core.Utilities.MultipleSymmetricKeySecurityToken.md) 
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md) 
