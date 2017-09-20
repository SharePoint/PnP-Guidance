# ListExtensions.GetListByUrl Method  
 Get list by using Url   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static List GetListByUrl(this Web web, String webRelativeUrl, params Expression<Func<List, Object>>[] expressions)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web (site) to be processed  

  

#### webRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Url of list relative to the web (site), e.g. lists/testlist  

  

#### expressions  
&emsp;&emsp;Type: System.Linq.Expressions.Expression&lt;System.Func&lt;Microsoft.SharePoint.Client.List, System.Object&gt;&gt;[]  
&emsp;&emsp;Additional list of lambda expressions of properties to load alike l => l.BaseType  

  

### Return Value
Type: List  
Returns list if found, null if no list is found.  


## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
