# YammerUtility.CreateYammerGroup Method  
 Can be used to create Yammer group to the Yammer network   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static YammerGroup CreateYammerGroup(String groupName, Boolean isPrivate, String accessToken)
```
### Parameters
#### groupName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Creates yammer group with given name  

  

#### isPrivate  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Sets yammer groups as private if the value is true. Otherwise sets as public group  

  

#### accessToken  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;accessToken will have all the required permissions to update or retrieve data to Yammer on behalf of the user  

  

### Return Value
Type: [YammerGroup](OfficeDevPnP.Core.Entities.YammerGroup.md)  
Returns YammerGroup created  


## See also
- [YammerUtility](OfficeDevPnP.Core.Utilities.YammerUtility.md) 
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md) 
