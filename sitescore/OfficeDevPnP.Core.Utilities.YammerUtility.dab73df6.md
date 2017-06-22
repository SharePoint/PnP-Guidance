# YammerUtility.CreateYammerGroupDiscussionPartXml Method  
 Constructs the webpart XML for yammer group needed to inject as Yammer web part to SharePoint page   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static string CreateYammerGroupDiscussionPartXml(String yammerNetworkName, Int32 yammerGroupId, Boolean showHeader, Boolean showFooter, Boolean useSSO = True)
```
### Parameters
#### yammerNetworkName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Yammer network name  

  

#### yammerGroupId  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Group ID  

  

#### showHeader  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Shows header based on value  

  

#### showFooter  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Shows footer based on value  

  

#### (optional) useSSO  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;uses given Single Sign-on information to create webpart  

  

### Return Value
Type: string  
The constructed web part XML  


## See also
- [YammerUtility](OfficeDevPnP.Core.Utilities.YammerUtility.md) 
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md) 
