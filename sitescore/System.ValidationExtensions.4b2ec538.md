# ValidationExtensions.ValidateNotNullOrEmpty Method  
 Validates an object for not being null or not being the default value   

**Namespace:** [System](System.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void ValidateNotNullOrEmpty<T>(this T input, String variableName)
```
### Parameters
#### input  
&emsp;&emsp;Type: T  
&emsp;&emsp;The objec tto check  

  

#### variableName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The name of the variable name to report in the error  

  

### Return Value
Type: void  

## See also
- [ValidationExtensions](System.ValidationExtensions.md) 
- System.ArgumentException
- System.ArgumentNullException
- [System](System.md) 
