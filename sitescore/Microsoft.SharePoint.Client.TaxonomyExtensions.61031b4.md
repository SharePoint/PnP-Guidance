# TaxonomyExtensions.CreateTaxonomyField Method  
 Can be used to create taxonomy field remotely in a list.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Field CreateTaxonomyField(this List list, TaxonomyFieldCreationInformation fieldCreationInformation)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;List to be processed  

  

#### fieldCreationInformation  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Entities.TaxonomyFieldCreationInformation](OfficeDevPnP.Core.Entities.TaxonomyFieldCreationInformation.md)  
&emsp;&emsp;Creation information of the field  

  

### Return Value
Type: Field  
New taxonomy field  


## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
