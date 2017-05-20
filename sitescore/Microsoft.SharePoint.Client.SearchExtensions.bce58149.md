# SearchExtensions.ExportSearchSettings Method  
 Exports the search settings to file.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void ExportSearchSettings(this ClientContext context, String exportFilePath, SearchObjectLevel searchSettingsExportLevel)
```
### Parameters
#### context  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ClientContext  
&emsp;&emsp;Context for SharePoint objects and operations  

  

#### exportFilePath  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Path where to export the search settings  

  

#### searchSettingsExportLevel  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Search.Administration.SearchObjectLevel  
&emsp;&emsp;Search settings export level Reference: http://msdn.microsoft.com/en-us/library/microsoft.sharepoint.client.search.administration.searchobjectlevel(v=office.15).aspx   

  

### Return Value
Type: void  

## See also
- [SearchExtensions](Microsoft.SharePoint.Client.SearchExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
