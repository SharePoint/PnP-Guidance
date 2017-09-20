# ClientSideWebPart.Import Method  
Imports a  [OfficeDevPnP.Core.Pages.ClientSideComponent](OfficeDevPnP.Core.Pages.ClientSideComponent.md)  to use it as base for configuring the client side web part instance  

**Namespace:** [OfficeDevPnP.Core.Pages](OfficeDevPnP.Core.Pages.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public void Import(ClientSideComponent component, Func<String, String> clientSideWebPartPropertiesUpdater)
```
### Parameters
#### component  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Pages.ClientSideComponent](OfficeDevPnP.Core.Pages.ClientSideComponent.md)  
&emsp;&emsp; to import  

  

#### (optional) clientSideWebPartPropertiesUpdater  
&emsp;&emsp;Type: System.Func&lt;System.String, System.String&gt;  
&emsp;&emsp;Function callback that allows you to manipulate the client side web part properties after import  

  

### Return Value
Type: void  

## See also
- [ClientSideWebPart](OfficeDevPnP.Core.Pages.ClientSideWebPart.md) 
- [OfficeDevPnP.Core.Pages.ClientSideComponent](OfficeDevPnP.Core.Pages.ClientSideComponent.md)
- [OfficeDevPnP.Core.Pages](OfficeDevPnP.Core.Pages.md) 
