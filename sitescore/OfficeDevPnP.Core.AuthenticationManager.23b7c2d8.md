# AuthenticationManager.RefreshADFSUserNameMixedAuthenticatedContext Method  
 Refreshes the SharePoint FedAuth cookie   

**Namespace:** [OfficeDevPnP.Core](OfficeDevPnP.Core.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public void RefreshADFSUserNameMixedAuthenticatedContext(String siteUrl, String user, String password, String domain, String sts, String idpId, Int32 logonTokenCacheExpirationWindow = 10)
```
### Parameters
#### siteUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Url of the SharePoint site that's secured via ADFS  

  

#### user  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the user (e.g. administrator)   

  

#### password  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Password of the user  

  

#### domain  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Windows domain of the user  

  

#### sts  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Hostname of the ADFS server (e.g. sts.company.com)  

  

#### idpId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Identifier of the ADFS relying party that we're hitting  

  

#### (optional) logonTokenCacheExpirationWindow  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Optioanlly provide the value of the SharePoint STS logonTokenCacheExpirationWindow. Defaults to 10 minutes.  

  

### Return Value
Type: void  

## See also
- [AuthenticationManager](OfficeDevPnP.Core.AuthenticationManager.md) 
- [OfficeDevPnP.Core](OfficeDevPnP.Core.md) 
