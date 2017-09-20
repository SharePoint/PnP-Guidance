# FieldAndContentTypeExtensions.FieldExistsById Method  
 Returns if the field is found   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool FieldExistsById(this Web web, Guid fieldId, Boolean searchInSiteHierarchy = False)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site. Site columns should be created to root site.  

  

#### fieldId  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;Guid for the field ID  

  

#### (optional) searchInSiteHierarchy  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;If true, search parent sites and root site  

  

### Return Value
Type: bool  
True or false depending on the field existence  


## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
