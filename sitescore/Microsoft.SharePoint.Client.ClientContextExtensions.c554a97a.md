# ClientContextExtensions.GetAccessToken Method  
 Gets an access token from a Microsoft.SharePoint.Client.ClientContext instance. Only works when using an add-in or app-only authentication flow.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static string GetAccessToken(this ClientRuntimeContext clientContext)
```
### Parameters
#### clientContext  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ClientRuntimeContext  
&emsp;&emsp; instance to obtain an access token for  

  

### Return Value
Type: string  
Access token for the given Microsoft.SharePoint.Client.ClientContext instance  


## See also
- [ClientContextExtensions](Microsoft.SharePoint.Client.ClientContextExtensions.md) 
- Microsoft.SharePoint.Client.ClientContext
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
