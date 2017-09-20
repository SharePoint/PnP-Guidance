# NavigationExtensions.GetEditableNavigationTermSet Method  
 Returns an editable version of the Global Navigation TermSet for a web site   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static NavigationTermSet GetEditableNavigationTermSet(this Web web, ManagedNavigationKind navigationKind)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The target web.  

  

#### navigationKind  
&emsp;&emsp;Type: [Microsoft.SharePoint.Client.ManagedNavigationKind](Microsoft.SharePoint.Client.ManagedNavigationKind.md)  
&emsp;&emsp;Declares whether to look for Current or Global Navigation  

  

### Return Value
Type: NavigationTermSet  
The editable Global Navigation TermSet  


## See also
- [NavigationExtensions](Microsoft.SharePoint.Client.NavigationExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
