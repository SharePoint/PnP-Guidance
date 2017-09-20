# ClientObjectExtensions.IsObjectPropertyInstantiated Method  
 Check if a property is instantiated on a object   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool IsObjectPropertyInstantiated<T>(this T clientObject, Expression<Func<T, Object>> propertySelector) where T : ClientObject
```
### Parameters
#### clientObject  
&emsp;&emsp;Type: T  
&emsp;&emsp;Object to operate on  

  

#### propertySelector  
&emsp;&emsp;Type: System.Linq.Expressions.Expression&lt;System.Func&lt;T, System.Object&gt;&gt;  
&emsp;&emsp;Lamda expression containing the properties to check (e.g. w => w.HasUniqueRoleAssignments)  

  

### Return Value
Type: bool  
True if the property is instantiated, false otherwise  


## See also
- [ClientObjectExtensions](Microsoft.SharePoint.Client.ClientObjectExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
