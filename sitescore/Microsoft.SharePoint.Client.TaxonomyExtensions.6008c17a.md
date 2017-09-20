# TaxonomyExtensions.CreateTaxonomyField Method  
 Can be used to create taxonomy field remotely to web.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Field CreateTaxonomyField(this Web web, TaxonomyFieldCreationInformation fieldCreationInformation)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### fieldCreationInformation  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Entities.TaxonomyFieldCreationInformation](OfficeDevPnP.Core.Entities.TaxonomyFieldCreationInformation.md)  
&emsp;&emsp;Creation Information of the field  

  

### Return Value
Type: Field  
New taxonomy field  


## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
