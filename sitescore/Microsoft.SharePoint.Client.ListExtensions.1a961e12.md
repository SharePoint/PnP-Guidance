# ListExtensions.CreateView Method  
 Create view to existing list   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static View CreateView(this List list, String viewName, ViewType viewType, String[] viewFields, UInt32 rowLimit, Boolean setAsDefault, String query, Boolean personal = False, Boolean paged = False)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;List to process  

  

#### viewName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the view  

  

#### viewType  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ViewType  
&emsp;&emsp;Type of the view  

  

#### viewFields  
&emsp;&emsp;Type: System.String[]  
&emsp;&emsp;Fields of the view  

  

#### rowLimit  
&emsp;&emsp;Type: System.UInt32  
&emsp;&emsp;Row limit of the view  

  

#### setAsDefault  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Set as default view  

  

#### (optional) query  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Query for view creation  

  

#### (optional) personal  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Personal View  

  

#### (optional) paged  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Paged view  

  

### Return Value
Type: View  

## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
