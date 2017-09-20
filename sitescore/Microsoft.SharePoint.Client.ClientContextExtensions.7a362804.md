# ClientContextExtensions.GetSiteCollectionContext Method  
 Gets a site collection context for the passed web. This site collection client context uses the same credentials as the passed client context   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static ClientContext GetSiteCollectionContext(this ClientRuntimeContext clientContext)
```
### Parameters
#### clientContext  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ClientRuntimeContext  
&emsp;&emsp;Client context to take the credentials from  

  

### Return Value
Type: ClientContext  
A site collection client context object for the site collection  


## See also
- [ClientContextExtensions](Microsoft.SharePoint.Client.ClientContextExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
