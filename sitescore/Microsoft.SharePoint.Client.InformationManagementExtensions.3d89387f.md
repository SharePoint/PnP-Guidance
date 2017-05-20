# InformationManagementExtensions.GetSiteExpirationDate Method  
 Gets the site expiration date   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static DateTime GetSiteExpirationDate(this Web web)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web to operate on  

  

### Return Value
Type: DateTime  
DateTime value holding the expiration date, DateTime.MinValue in case there was no policy applied  


## See also
- [InformationManagementExtensions](Microsoft.SharePoint.Client.InformationManagementExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
