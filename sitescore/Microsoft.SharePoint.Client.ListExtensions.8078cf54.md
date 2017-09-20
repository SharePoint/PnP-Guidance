# ListExtensions.GetListByTitle Method  
 Get list by using Title   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static List GetListByTitle(this Web web, String listTitle, params Expression<Func<List, Object>>[] expressions)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### listTitle  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Title of the list to return  

  

#### expressions  
&emsp;&emsp;Type: System.Linq.Expressions.Expression&lt;System.Func&lt;Microsoft.SharePoint.Client.List, System.Object&gt;&gt;[]  
&emsp;&emsp;Additional list of lambda expressions of properties to load alike l => l.BaseType  

  

### Return Value
Type: List  
Loaded list instance matching to title or null  


## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- System.ArgumentException
- System.ArgumentNullException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
