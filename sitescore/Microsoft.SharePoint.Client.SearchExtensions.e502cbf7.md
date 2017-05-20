# SearchExtensions.ImportSearchSettings Method  
 Imports search settings from file.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void ImportSearchSettings(this ClientContext context, String searchSchemaImportFilePath, SearchObjectLevel searchSettingsImportLevel)
```
### Parameters
#### context  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ClientContext  
&emsp;&emsp;Context for SharePoint objects and operations  

  

#### searchSchemaImportFilePath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Search schema xml file path  

  

#### searchSettingsImportLevel  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Search.Administration.SearchObjectLevel  
&emsp;&emsp;Search settings import level Reference: http://msdn.microsoft.com/en-us/library/microsoft.sharepoint.client.search.administration.searchobjectlevel(v=office.15).aspx   

  

### Return Value
Type: void  

## See also
- [SearchExtensions](Microsoft.SharePoint.Client.SearchExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
