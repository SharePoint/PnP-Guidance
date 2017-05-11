# ClientObjectExtensions.EnsureProperty Method  
 Ensures that particular property is loaded on the Microsoft.SharePoint.Client.ClientObject and immediately returns this property   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static TResult EnsureProperty(T clientObject, Expression<Func<T, TResult>> propertySelector)
```
### Parameters
#### clientObject  
&emsp;&emsp;Type: T  
&emsp;&emsp; Ensures that particular property is loaded on the Microsoft.SharePoint.Client.ClientObject and immediately returns this property   

  

#### propertySelector  
&emsp;&emsp;Type: System.Linq.Expressions.Expression<System.Func<T, TResult>>  
&emsp;&emsp;Lamda expression containing the property to ensure (e.g. w => w.HasUniqueRoleAssignments)  

  

### Return Value
Type: TResult  
Property value  


## Remarks
  
## See also
- [ClientObjectExtensions](Microsoft.SharePoint.Client.ClientObjectExtensions.md) 
- Microsoft.SharePoint.Client.ClientObject
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
