# ListExtensions.GetViewById Method  
 Gets a view by Id   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static View GetViewById(this List list, Guid id, params Expression<Func<View, Object>>[] expressions)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;List to process  

  

#### id  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;Id to the view to extract  

  

#### expressions  
&emsp;&emsp;Type: System.Linq.Expressions.Expression&lt;System.Func&lt;Microsoft.SharePoint.Client.View, System.Object&gt;&gt;[]  
&emsp;&emsp;List of lambda expressions of properties to load when retrieving the object  

  

### Return Value
Type: View  
returns null if not found  


## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
