# YammerUtility.CreateYammerOpenGraphDiscussionPartXml Method  
 Constructs web part definition for Open Graph discussion web part definition   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static string CreateYammerOpenGraphDiscussionPartXml(String yammerNetworkName, String url, Boolean showHeader, Boolean showFooter, String postTitle = "", String postImageUrl = "", Boolean useSso = True, String groupId = "")
```
### Parameters
#### yammerNetworkName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Yammer network name  

  

#### url  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Yammer url  

  

#### showHeader  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Shows header based on value  

  

#### showFooter  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Shows footer based on value  

  

#### (optional) postTitle  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;creates webpart with given post title  

  

#### (optional) postImageUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;creates webpart with given post title  

  

#### (optional) useSso  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;uses given Single Sign-on information to create webpart  

  

#### (optional) groupId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;yammer group id  

  

### Return Value
Type: string  
The constructed Open Graph Discussion Part XML  


## See also
- [YammerUtility](OfficeDevPnP.Core.Utilities.YammerUtility.md) 
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md) 
