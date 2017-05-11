# ListExtensions.GetPropertyBagValueInt Method  
 Get int typed property bag value. If does not contain, returns default value.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Nullable<Int32> GetPropertyBagValueInt(List list, String key, Int32 defaultValue)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;List to read the property bag value from  

  

#### key  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Key of the property bag entry to return  

  

#### defaultValue  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp; Get int typed property bag value. If does not contain, returns default value.   

  

### Return Value
Type: Nullable<Int32>  
Value of the property bag entry as integer  


## Remarks
  
## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
