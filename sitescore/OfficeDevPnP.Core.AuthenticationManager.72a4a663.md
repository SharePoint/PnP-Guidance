# AuthenticationManager.GetAppOnlyAuthenticatedContext Method  
 Returns an app only ClientContext object   

**Namespace:** [OfficeDevPnP.Core](OfficeDevPnP.Core.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public ClientContext GetAppOnlyAuthenticatedContext(String siteUrl, String realm, String appId, String appSecret, String acsHostUrl = "accesscontrol.windows.net", String globalEndPointPrefix = "accounts")
```
### Parameters
#### siteUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Site for which the ClientContext object will be instantiated  

  

#### realm  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Realm of the environment (tenant) that requests the ClientContext object  

  

#### appId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Application ID which is requesting the ClientContext object  

  

#### appSecret  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Application secret of the Application which is requesting the ClientContext object  

  

#### (optional) acsHostUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Azure ACS host, defaults to accesscontrol.windows.net but internal pre-production environments use other hosts  

  

#### (optional) globalEndPointPrefix  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Azure ACS endpoint prefix, defaults to accounts but internal pre-production environments use other prefixes  

  

### Return Value
Type: ClientContext  
ClientContext to be used by CSOM code  


## See also
- [AuthenticationManager](OfficeDevPnP.Core.AuthenticationManager.md) 
- [OfficeDevPnP.Core](OfficeDevPnP.Core.md) 
