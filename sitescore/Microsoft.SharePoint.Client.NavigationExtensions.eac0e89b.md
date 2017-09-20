# NavigationExtensions.GetCustomActions Method  
 Returns all custom actions in a web   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static IEnumerable<UserCustomAction> GetCustomActions(this Web web, params Expression<Func<UserCustomAction, Object>>[] expressions)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The web to process  

  

#### expressions  
&emsp;&emsp;Type: System.Linq.Expressions.Expression&lt;System.Func&lt;Microsoft.SharePoint.Client.UserCustomAction, System.Object&gt;&gt;[]  
&emsp;&emsp;List of lambda expressions of properties to load when retrieving the object  

  

### Return Value
Type: IEnumerable<UserCustomAction>  
Returns all custom actions  


## See also
- [NavigationExtensions](Microsoft.SharePoint.Client.NavigationExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
