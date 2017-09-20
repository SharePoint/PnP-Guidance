# FieldAndContentTypeExtensions.CreateFieldsFromXML Method  
 Creates field from xml structure which follows the classic feature framework structure   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void CreateFieldsFromXML(this Web web, XDocument xDocument)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site. Site columns should be created to root site.  

  

#### xDocument  
&emsp;&emsp;Type: System.Xml.Linq.XDocument  
&emsp;&emsp;Actual XML document  

  

### Return Value
Type: void  

## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
