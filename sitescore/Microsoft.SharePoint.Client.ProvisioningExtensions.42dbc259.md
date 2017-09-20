# ProvisioningExtensions.ProvisionElementFile Method  
 Provisions the items defined by the specified Elements (CAML) file; currently only supports modules (files).   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void ProvisionElementFile(this Web web, String path)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to provision the elements to  

  

#### path  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Path to the XML file containing the Elements CAML defintion  

  

### Return Value
Type: void  

## See also
- [ProvisioningExtensions](Microsoft.SharePoint.Client.ProvisioningExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
