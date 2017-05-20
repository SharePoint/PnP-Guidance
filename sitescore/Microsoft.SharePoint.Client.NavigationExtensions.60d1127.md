# NavigationExtensions.IsManagedNavigationEnabled Method  
 Determines whether the current Web has the managed navigation enabled   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool IsManagedNavigationEnabled(this Web web, ManagedNavigationKind navigationKind)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The target web.  

  

#### navigationKind  
&emsp;&emsp;Type: [Microsoft.SharePoint.Client.ManagedNavigationKind](Microsoft.SharePoint.Client.ManagedNavigationKind.md)  
&emsp;&emsp;The kind of navigation (Current or Global).  

  

### Return Value
Type: bool  
A boolean result of the test.  


## See also
- [NavigationExtensions](Microsoft.SharePoint.Client.NavigationExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
