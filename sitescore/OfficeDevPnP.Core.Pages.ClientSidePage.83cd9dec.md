# ClientSidePage.Load Method  
 Loads an existint SharePoint client side page   

**Namespace:** [OfficeDevPnP.Core.Pages](OfficeDevPnP.Core.Pages.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static ClientSidePage Load(ClientContext cc, String pageName)
```
### Parameters
#### cc  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ClientContext  
&emsp;&emsp;ClientContext object used to load the page  

  

#### pageName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the page (e.g. mypage.aspx) to load  

  

### Return Value
Type: [ClientSidePage](OfficeDevPnP.Core.Pages.ClientSidePage.md)  
A  [OfficeDevPnP.Core.Pages.ClientSidePage](OfficeDevPnP.Core.Pages.ClientSidePage.md)  instance for the given page  


## See also
- [ClientSidePage](OfficeDevPnP.Core.Pages.ClientSidePage.md) 
- [OfficeDevPnP.Core.Pages.ClientSidePage](OfficeDevPnP.Core.Pages.ClientSidePage.md)
- [OfficeDevPnP.Core.Pages](OfficeDevPnP.Core.Pages.md) 
