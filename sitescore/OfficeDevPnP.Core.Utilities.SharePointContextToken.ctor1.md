# SharePointContextToken.SharePointContextToken members 
 Constructor for SharePointContextToken class   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public SharePointContextToken(string issuer, string audience, DateTime validFrom, DateTime validTo, IEnumerable<JsonWebTokenClaim> claims)
```
### Parameters
#### issuer  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Token Issuer  


#### audience  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Token Audience  


#### validFrom  
&emsp;&emsp;Type: System.DateTime  
&emsp;&emsp;Validity start date for token  


#### validTo  
&emsp;&emsp;Type: System.DateTime  
&emsp;&emsp;Validity end date for token  


#### claims  
&emsp;&emsp;Type: System.Collections.Generic.IEnumerable<SharePointPnP.IdentityModel.Extensions.S2S.Tokens.JsonWebTokenClaim>  
&emsp;&emsp;IEnumerable of JsonWebTokenClaim object  


## See also
- [SharePointContextToken](OfficeDevPnP.Core.Utilities.SharePointContextToken.md)
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)
