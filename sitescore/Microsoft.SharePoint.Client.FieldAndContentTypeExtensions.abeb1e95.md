# FieldAndContentTypeExtensions.CreateFieldsFromXMLString Method  
 Creates fields from feature element xml file schema. XML file can contain one or many field definitions created using classic feature framework structure.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void CreateFieldsFromXMLString(this Web web, String xmlStructure)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site. Site columns should be created to root site.  

  

#### xmlStructure  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;XML structure in string format  

  

### Return Value
Type: void  

## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
