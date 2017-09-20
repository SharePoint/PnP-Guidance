# NavigationExtensions.AddCustomAction Method  
 Adds custom action to a web. If the CustomAction exists the item will be updated. Setting CustomActionEntity.Remove == true will delete the CustomAction.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool AddCustomAction(this Web web, CustomActionEntity customAction)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### customAction  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Entities.CustomActionEntity](OfficeDevPnP.Core.Entities.CustomActionEntity.md)  
&emsp;&emsp;Information about the custom action be added or deleted  

  

### Return Value
Type: bool  
True if action was successfull  


## Examples
```C#
var editAction = new CustomActionEntity()
{
   Title = "Edit Site Classification",
   Description = "Manage business impact information for site collection or sub sites.",
   Sequence = 1000,
   Group = "SiteActions",
   Location = "Microsoft.SharePoint.StandardMenu",
   Url = EditFormUrl,
   ImageUrl = EditFormImageUrl,
   Rights = new BasePermissions(),
};
editAction.Rights.Set(PermissionKind.ManageWeb);
web.AddCustomAction(editAction);
```

## See also
- [NavigationExtensions](Microsoft.SharePoint.Client.NavigationExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
