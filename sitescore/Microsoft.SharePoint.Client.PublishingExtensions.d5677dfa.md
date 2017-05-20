# PublishingExtensions.AddPublishingPage Method  
 Adds the publishing page.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AddPublishingPage(this Web web, String pageName, String pageTemplateName, String title, Boolean publish = False, Folder folder, Nullable<DateTime> startDate, Nullable<DateTime> endDate, Boolean schedule = False)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The web.  

  

#### pageName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the page.  

  

#### pageTemplateName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the page template/layout excluded the .aspx file extension.  

  

#### (optional) title  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The title of the target publishing page.  

  

#### (optional) publish  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Should the page be published or not?  

  

#### (optional) folder  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Folder  
&emsp;&emsp;The target folder for the page, within the Pages library.  

  

#### (optional) startDate  
&emsp;&emsp;Type: System.Nullable&lt;System.DateTime&gt;  
&emsp;&emsp;Start date for scheduled publishing.  

  

#### (optional) endDate  
&emsp;&emsp;Type: System.Nullable&lt;System.DateTime&gt;  
&emsp;&emsp;End date for scheduled publishing.  

  

#### (optional) schedule  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Defines whether to define a schedule or not.  

  

### Return Value
Type: void  

## See also
- [PublishingExtensions](Microsoft.SharePoint.Client.PublishingExtensions.md) 
- System.ArgumentNullException
- System.ArgumentException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
