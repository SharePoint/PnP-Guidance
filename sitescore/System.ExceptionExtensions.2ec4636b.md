# ExceptionExtensions.ToDetailedString Method  
 Returns exception based on ClientRunTimeContext and ExceptionOptions objects   

**Namespace:** [System](System.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static string ToDetailedString(this Exception exception, ClientRuntimeContext cc, ExceptionOptions options)
```
### Parameters
#### exception  
&emsp;&emsp;Type: System.Exception  
&emsp;&emsp;Exception object  

  

#### cc  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ClientRuntimeContext  
&emsp;&emsp;ClientRuntimeContext object  

  

#### options  
&emsp;&emsp;Type: [System.ExceptionOptions](System.ExceptionOptions.md)  
&emsp;&emsp;ExceptionOptions object  

  

### Return Value
Type: string  
Returns exception as a string  


## See also
- [ExceptionExtensions](System.ExceptionExtensions.md) 
- [System](System.md) 
