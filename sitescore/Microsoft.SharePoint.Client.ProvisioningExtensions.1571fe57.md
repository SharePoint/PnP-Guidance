# ProvisioningExtensions.ProvisionElementXml Method  
 Provisions the items defined by the specified Elements (CAML) XML; currently only supports modules (files).   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void ProvisionElementXml(this Web web, String baseFolder, XElement elementsXml)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to provision the elements to  

  

#### baseFolder  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Base local folder to find any referenced items, e.g. files  

  

#### elementsXml  
&emsp;&emsp;Type: System.Xml.Linq.XElement  
&emsp;&emsp;Elements (CAML) XML element that defines the items to provision; currently only supports modules (files)  

  

### Return Value
Type: void  

## See also
- [ProvisioningExtensions](Microsoft.SharePoint.Client.ProvisioningExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
