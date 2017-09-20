# WebExtensions.GetPropertyBagValueInt Method  
 Get int typed property bag value. If does not contain, returns default value.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Nullable<Int32> GetPropertyBagValueInt(this Web web, String key, Int32 defaultValue)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to read the property bag value from  

  

#### key  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Key of the property bag entry to return  

  

#### defaultValue  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp; Get int typed property bag value. If does not contain, returns default value.   

  

### Return Value
Type: Nullable<Int32>  
Value of the property bag entry as integer  


## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
