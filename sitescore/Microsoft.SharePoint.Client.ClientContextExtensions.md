# ClientContextExtensions Class
 Class that deals with cloning client context object, getting access token and validates server version 

 Class that holds the deprecated clientcontext methods   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class ClientContextExtensions
```
## Extension Methods
|**Name**|**Description**|
|:-----|:-----|
| [Clone(ClientRuntimeContext, String)](Microsoft.SharePoint.Client.ClientContextExtensions.496ce2a9.md) | Clones a ClientContext object while "taking over" the security context of the existing ClientContext instance
| [Clone(ClientRuntimeContext, Uri)](Microsoft.SharePoint.Client.ClientContextExtensions.24377799.md) | Clones a ClientContext object while "taking over" the security context of the existing ClientContext instance
| [CreateSiteAsync(ClientContext, CommunicationSiteCollectionCreationInformation)](Microsoft.SharePoint.Client.ClientContextExtensions.d7359633.md) | BETA: Creates a Communication Site Collection
| [CreateSiteAsync(ClientContext, TeamSiteCollectionCreationInformation)](Microsoft.SharePoint.Client.ClientContextExtensions.369b07fa.md) | BETA: Creates a Team Site Collection
| [ExecuteQueryRetry(ClientRuntimeContext, Int32, Int32, String)](Microsoft.SharePoint.Client.ClientContextExtensions.48ec5823.md) | Executes the current set of data retrieval queries and method invocations and retries it if needed.
| [GetAccessToken(ClientRuntimeContext)](Microsoft.SharePoint.Client.ClientContextExtensions.c554a97a.md) |  Gets an access token from a Microsoft.SharePoint.Client.ClientContext instance. Only works when using an add-in or app-only authentication flow. 
| [GetRequestDigest(ClientContext)](Microsoft.SharePoint.Client.ClientContextExtensions.46268e83.md) | Returns the request digest from the current session/site
| [GetSiteCollectionContext(ClientRuntimeContext)](Microsoft.SharePoint.Client.ClientContextExtensions.7a362804.md) | Gets a site collection context for the passed web. This site collection client context uses the same credentials as the passed client context
| [HasMinimalServerLibraryVersion(ClientRuntimeContext, String)](Microsoft.SharePoint.Client.ClientContextExtensions.972110cc.md) | Checks the server library version of the context for a minimally required version
| [HasMinimalServerLibraryVersion(ClientRuntimeContext, Version)](Microsoft.SharePoint.Client.ClientContextExtensions.136acdfc.md) | Checks the server library version of the context for a minimally required version
| [IsAppOnly(ClientRuntimeContext)](Microsoft.SharePoint.Client.ClientContextExtensions.c747dff1.md) | Checks if the used ClientContext is app-only
## See also
- Microsoft.SharePoint.Client.ClientContext
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)
