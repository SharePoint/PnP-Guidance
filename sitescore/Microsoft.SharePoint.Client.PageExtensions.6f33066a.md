# PageExtensions.AddClientSidePage Method  
 Adds a client side "modern" page to a "classic" or "modern" site   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static ClientSidePage AddClientSidePage(Web web, String pageName, Boolean alreadyPersist)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to add the page to  

  

#### pageName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name (e.g. demo.aspx) of the page to be added  

  

#### (optional) alreadyPersist  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Already persist the created, empty, page before returning the instantiated instance  

  

### Return Value
Type: ClientSidePage  
A  [OfficeDevPnP.Core.Pages.ClientSidePage](OfficeDevPnP.Core.Pages.ClientSidePage.md)  instance  


## Remarks
  
## See also
- [PageExtensions](Microsoft.SharePoint.Client.PageExtensions.md) 
- [OfficeDevPnP.Core.Pages.ClientSidePage](OfficeDevPnP.Core.Pages.ClientSidePage.md)
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
