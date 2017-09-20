# CAML.ViewQuery Method  
 Root &lt;View&gt; and &lt;Query&gt; nodes.   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static string ViewQuery(ViewScope scope, String whereClause = "", String orderByClause = "", String viewFields = "", Int32 rowLimit = 100)
```
### Parameters
#### scope  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ViewScope  
&emsp;&emsp;View scope  

  

#### (optional) whereClause  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;<Where> node.  

  

#### (optional) orderByClause  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;<OrderBy> node.  

  

#### (optional) viewFields  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;<ViewFields> node.  

  

#### (optional) rowLimit  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;<RowLimit> node.  

  

### Return Value
Type: string  
String to be used in CAML queries  


## See also
- [CAML](OfficeDevPnP.Core.Utilities.CAML.md) 
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md) 
