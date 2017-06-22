# CAML.FieldValue Method  
 Creates both a &lt;FieldRef&gt; and &lt;Value&gt; nodes combination for Where clauses.   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static string FieldValue(Guid fieldId, String fieldValueType, String value, String additionalFieldRefParams = "")
```
### Parameters
#### fieldId  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;Id of the field  

  

#### fieldValueType  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Value type of the field  

  

#### value  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Value of the field  

  

#### (optional) additionalFieldRefParams  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Additional FieldRef Parameters  

  

### Return Value
Type: string  
Returns FieldValue string to be used in CAML queries  


## See also
- [CAML](OfficeDevPnP.Core.Utilities.CAML.md) 
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md) 
