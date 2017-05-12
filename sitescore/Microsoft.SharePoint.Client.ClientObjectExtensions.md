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
| [EnsureProperties(T, Expression&lt;Func&lt;T, Object&gt;&gt;[])](Microsoft.SharePoint.Client.ClientObjectExtensions.f3e7f8b2.md) |  Ensures that particular properties are loaded on the Microsoft.SharePoint.Client.ClientObject 
| [EnsureProperty(T, Expression&lt;Func&lt;T, TResult&gt;&gt;)](Microsoft.SharePoint.Client.ClientObjectExtensions.82424018.md) |  Ensures that particular property is loaded on the Microsoft.SharePoint.Client.ClientObject and immediately returns this property 
| [IsObjectPropertyInstantiated(T, Expression&lt;Func&lt;T, Object&gt;&gt;)](Microsoft.SharePoint.Client.ClientObjectExtensions.e1e682e5.md) | Check if a property is instantiated on a object
| [IsPropertyAvailable(T, Expression&lt;Func&lt;T, Object&gt;&gt;)](Microsoft.SharePoint.Client.ClientObjectExtensions.12af663c.md) | Check if a property is available on a object
| [ServerObjectIsNull(T)](Microsoft.SharePoint.Client.ClientObjectExtensions.bd54c126.md) | Checks if the ClientObject is null
| [ToUntypedPropertyExpression(Expression&lt;Func&lt;TInput, TOutput&gt;&gt;)](Microsoft.SharePoint.Client.ClientObjectExtensions.730653d1.md) | Converts generic Expression&lt;Func&lt;TInput, TOutput&gt;&gt; to Expression with object return type - Expression&lt;Func&lt;TInput, object&gt;&gt;
| [ToUntypedStaticMethodCallExpression(Expression&lt;Func&lt;TInput, TOutput&gt;&gt;)](Microsoft.SharePoint.Client.ClientObjectExtensions.4db1f274.md) | Converts generic Expression&lt;Func&lt;TInput, TOutput&gt;&gt; to Expression with object return type - Expression&lt;Func&lt;TInput, object&gt;&gt;
## See also
- Microsoft.SharePoint.Client.ClientObject
- System.Linq.Expressions.Expression
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)
