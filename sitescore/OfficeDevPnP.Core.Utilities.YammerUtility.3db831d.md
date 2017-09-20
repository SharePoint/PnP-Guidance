# YammerUtility.GetYammerGroupByName Method  
 Returns Yammer Group if group exists. If the group does not exist, returns null.   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static YammerGroup GetYammerGroupByName(String groupName, String accessToken)
```
### Parameters
#### groupName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Group name to search for  

  

#### accessToken  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;accessToken will have all the required permissions to update or retrieve data to Yammer on behalf of the user  

  

### Return Value
Type: [YammerGroup](OfficeDevPnP.Core.Entities.YammerGroup.md)  
Returns Yammer Group is group exists. If group does not exists, returns null.  


## See also
- [YammerUtility](OfficeDevPnP.Core.Utilities.YammerUtility.md) 
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md) 
