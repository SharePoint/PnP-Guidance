# ListExtensions.GetPropertyBagValueString Method  
 Get string typed property bag value. If does not contain, returns given default value.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static string GetPropertyBagValueString(this List list, String key, String defaultValue)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;List to read the property bag value from  

  

#### key  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Key of the property bag entry to return  

  

#### defaultValue  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Default value of the property bag  

  

### Return Value
Type: string  
Value of the property bag entry as string  


## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
