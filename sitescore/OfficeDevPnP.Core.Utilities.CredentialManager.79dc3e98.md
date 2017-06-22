# CredentialManager.GetSharePointOnlineCredential Method  
 Returns a SharePoint Online Credential given a certain name. Add the credential in the Windows Credential Manager and create a new Windows Credential. Then add a new GENERIC Credential. The name parameter in the method maps to the Internet or network address field.   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static SharePointOnlineCredentials GetSharePointOnlineCredential(String name)
```
### Parameters
#### name  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name maps to internet or network address fields  

  

### Return Value
Type: SharePointOnlineCredentials  
Microsoft.SharePoint.Client.SharePointOnlineCredentials  


## See also
- [CredentialManager](OfficeDevPnP.Core.Utilities.CredentialManager.md) 
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md) 
