# FieldAndContentTypeExtensions.AddContentTypeToListById Method  
 Adds content type to list   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddContentTypeToListById(this Web web, String listTitle, String contentTypeId, Boolean defaultContent = False, Boolean searchContentTypeInSiteHierarchy = False)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### listTitle  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Title of the list  

  

#### contentTypeId  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Complete ID for the content type  

  

#### (optional) defaultContent  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Optionally make this the default content type  

  

#### (optional) searchContentTypeInSiteHierarchy  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;search for content type in site hierarchy  

  

### Return Value
Type: void  

## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
