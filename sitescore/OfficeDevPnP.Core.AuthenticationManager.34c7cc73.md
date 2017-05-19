# AuthenticationManager.GetNetworkCredentialAuthenticatedContext Method  
 Returns a SharePoint on-premises / SharePoint Online Dedicated ClientContext object   

**Namespace:** [OfficeDevPnP.Core](OfficeDevPnP.Core.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public ClientContext GetNetworkCredentialAuthenticatedContext(String siteUrl, String user, SecureString password, String domain)
```
### Parameters
#### siteUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Site for which the ClientContext object will be instantiated  

  

#### user  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;User to be used to instantiate the ClientContext object  

  

#### password  
&emsp;&emsp;Type: System.Security.SecureString  
&emsp;&emsp;Password (SecureString) of the user used to instantiate the ClientContext object  

  

#### domain  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Domain of the user used to instantiate the ClientContext object  

  

### Return Value
Type: ClientContext  
ClientContext to be used by CSOM code  


## See also
- [AuthenticationManager](OfficeDevPnP.Core.AuthenticationManager.md) 
- [OfficeDevPnP.Core](OfficeDevPnP.Core.md) 
