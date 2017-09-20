# ClientContextExtensions.HasMinimalServerLibraryVersion Method  
 Checks the server library version of the context for a minimally required version   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool HasMinimalServerLibraryVersion(this ClientRuntimeContext clientContext, String minimallyRequiredVersion)
```
### Parameters
#### clientContext  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ClientRuntimeContext  
&emsp;&emsp;clientContext to operate on  

  

#### minimallyRequiredVersion  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;provide version to validate  

  

### Return Value
Type: bool  
True if it has minimal required version, false otherwise  


## See also
- [ClientContextExtensions](Microsoft.SharePoint.Client.ClientContextExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
