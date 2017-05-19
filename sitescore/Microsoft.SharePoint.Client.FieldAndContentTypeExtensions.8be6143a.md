# FieldAndContentTypeExtensions.CreateField Method  
 Create field to web remotely   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Field CreateField(Web web, String fieldAsXml, Boolean executeQuery)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### fieldAsXml  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The XML declaration of SiteColumn definition  

  

#### (optional) executeQuery  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp; Create field to web remotely   

  

### Return Value
Type: Field  
The newly created field or existing field.  


## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
