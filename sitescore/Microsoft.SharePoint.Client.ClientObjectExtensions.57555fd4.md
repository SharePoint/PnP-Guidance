# ClientObjectExtensions.ToUntypedStaticMethodCallExpression Method  
 Converts generic  Expression&lt;Func&lt;TInput, TOutput&gt;&gt;  to Expression with object return type -  Expression&lt;Func&lt;TInput, object&gt;&gt;   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Expression<Func<TInput, Object>> ToUntypedStaticMethodCallExpression<TInput, TOutput>(this Expression<Func<TInput, TOutput>> expression)
```
### Parameters
#### expression  
&emsp;&emsp;Type: System.Linq.Expressions.Expression&lt;System.Func&lt;TInput, TOutput&gt;&gt;  
&emsp;&emsp; to convert   

  

### Return Value
Type: Expression<Func<TInput,  Object>>  
New Expression where return type is object and not generic  


## See also
- [ClientObjectExtensions](Microsoft.SharePoint.Client.ClientObjectExtensions.md) 
- System.Linq.Expressions.Expression
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
