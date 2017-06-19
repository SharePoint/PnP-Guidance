# WebExtensions.GetAppInstances Method  
 Returns all app instances   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static ClientObjectList<AppInstance> GetAppInstances(this Web web, params Expression<Func<AppInstance, Object>>[] expressions)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The site to process  

  

#### expressions  
&emsp;&emsp;Type: System.Linq.Expressions.Expression&lt;System.Func&lt;Microsoft.SharePoint.Client.AppInstance, System.Object&gt;&gt;[]  
&emsp;&emsp;List of lambda expressions of properties to load when retrieving the object  

  

### Return Value
Type: ClientObjectList<AppInstance>  
all app instances  


## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
