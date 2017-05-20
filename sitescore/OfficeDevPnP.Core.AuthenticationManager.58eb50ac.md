# AuthenticationManager.GetAppOnlyAuthenticatedContext Method  
 Returns an app only ClientContext object   

**Namespace:** [OfficeDevPnP.Core](OfficeDevPnP.Core.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public ClientContext GetAppOnlyAuthenticatedContext(String siteUrl, String appId, String appSecret, AzureEnvironment environment = 0)
```
### Parameters
#### siteUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Site for which the ClientContext object will be instantiated  

  

#### appId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Application ID which is requesting the ClientContext object  

  

#### appSecret  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Application secret of the Application which is requesting the ClientContext object  

  

#### (optional) environment  
&emsp;&emsp;Type: [OfficeDevPnP.Core.AzureEnvironment](OfficeDevPnP.Core.AzureEnvironment.md)  
&emsp;&emsp;SharePoint environment being used  

  

### Return Value
Type: ClientContext  
ClientContext to be used by CSOM code  


## See also
- [AuthenticationManager](OfficeDevPnP.Core.AuthenticationManager.md) 
- [OfficeDevPnP.Core](OfficeDevPnP.Core.md) 
