# NavigationExtensions.AddCustomAction Method  
 Adds custom action to a site collection. If the CustomAction exists the item will be updated. Setting CustomActionEntity.Remove == true will delete the CustomAction.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool AddCustomAction(this Site site, CustomActionEntity customAction)
```
### Parameters
#### site  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Site  
&emsp;&emsp;Site collection to be processed  

  

#### customAction  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Entities.CustomActionEntity](OfficeDevPnP.Core.Entities.CustomActionEntity.md)  
&emsp;&emsp;Information about the custom action be added or deleted  

  

### Return Value
Type: bool  
True if action was successfull  


## See also
- [NavigationExtensions](Microsoft.SharePoint.Client.NavigationExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
