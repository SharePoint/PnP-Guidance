# ClientObjectExtensions Class
  

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class ClientObjectExtensions
```
## Extension Methods
|**Name**|**Description**|
|:-----|:-----|
| [EnsureProperties(T, Expression<Func<T, Object>>[])](Microsoft.SharePoint.Client.ClientObjectExtensions.662d7ca7.md) |  Ensures that particular properties are loaded on the Microsoft.SharePoint.Client.ClientObject 
| [EnsureProperty(T, Expression<Func<T, TResult>>)](Microsoft.SharePoint.Client.ClientObjectExtensions.84242e1a.md) |  Ensures that particular property is loaded on the Microsoft.SharePoint.Client.ClientObject and immediately returns this property 
| [IsObjectPropertyInstantiated(T, Expression<Func<T, Object>>)](Microsoft.SharePoint.Client.ClientObjectExtensions.21ee3124.md) | Check if a property is instantiated on a object
| [IsPropertyAvailable(T, Expression<Func<T, Object>>)](Microsoft.SharePoint.Client.ClientObjectExtensions.18c63636.md) | Check if a property is available on a object
| [ServerObjectIsNull(T)](Microsoft.SharePoint.Client.ClientObjectExtensions.bd54c126.md) | Checks if the ClientObject is null
| [ToUntypedPropertyExpression(Expression<Func<TInput, TOutput>>)](Microsoft.SharePoint.Client.ClientObjectExtensions.966602f3.md) | Converts generic Expression&lt;Func&lt;TInput, TOutput&gt;&gt; to Expression with object return type - Expression&lt;Func&lt;TInput, object&gt;&gt;
| [ToUntypedStaticMethodCallExpression(Expression<Func<TInput, TOutput>>)](Microsoft.SharePoint.Client.ClientObjectExtensions.57555fd4.md) | Converts generic Expression&lt;Func&lt;TInput, TOutput&gt;&gt; to Expression with object return type - Expression&lt;Func&lt;TInput, object&gt;&gt;
## See also
- Microsoft.SharePoint.Client.ClientObject
- System.Linq.Expressions.Expression
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)
