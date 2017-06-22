# CredentialManager Class
 Class for getting and managing Credentials for SharePoint Online and SharePoint Onpremise   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class CredentialManager
```
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [GetCredential(String)](OfficeDevPnP.Core.Utilities.CredentialManager.9be51d8d.md) | Returns a NetworkCredential given a certain name. Add the credential in the Windows Credential Manager and create a new Windows Credential. Then add a new GENERIC Credential. The name parameter in the method maps to the Internet or network address field.
| [GetSharePointOnlineCredential(String)](OfficeDevPnP.Core.Utilities.CredentialManager.79dc3e98.md) | Returns a SharePoint Online Credential given a certain name. Add the credential in the Windows Credential Manager and create a new Windows Credential. Then add a new GENERIC Credential. The name parameter in the method maps to the Internet or network address field.
## See also
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)
