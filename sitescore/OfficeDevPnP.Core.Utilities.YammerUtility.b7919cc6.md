# YammerUtility.GetYammerGroupDiscussionPart Method  
 Creates web part entity with the Yammer group structure on it   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static WebPartEntity GetYammerGroupDiscussionPart(String yammerNetworkName, Int32 yammerGroupId, Boolean showHeader, Boolean showFooter)
```
### Parameters
#### yammerNetworkName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Yammer group network name  

  

#### yammerGroupId  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Yammer group id  

  

#### showHeader  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Shows header of webpart based on the value  

  

#### showFooter  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Shows footer of webpart based on value  

  

### Return Value
Type: [WebPartEntity](OfficeDevPnP.Core.Entities.WebPartEntity.md)  
Returns created WebPartEntity  


## See also
- [YammerUtility](OfficeDevPnP.Core.Utilities.YammerUtility.md) 
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md) 
