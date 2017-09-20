# PageExtensions.AddNavigationFriendlyUrl Method  
 Adds a user-friendly URL for a PublishingPage object.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static string AddNavigationFriendlyUrl(this PublishingPage page, Web web, String navigationTitle, String friendlyUrlSegment, NavigationTermSetItem editableParent, Boolean showInGlobalNavigation = True, Boolean showInCurrentNavigation = True)
```
### Parameters
#### page  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Publishing.PublishingPage  
&emsp;&emsp;The target page to add to managed navigation.  

  

#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The target web.  

  

#### navigationTitle  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The title for the navigation item.  

  

#### friendlyUrlSegment  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The user-friendly text to use as the URL segment.  

  

#### editableParent  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Publishing.Navigation.NavigationTermSetItem  
&emsp;&emsp;The parent NavigationTermSetItem object below which this new friendly URL should be created.  

  

#### (optional) showInGlobalNavigation  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Defines whether the navigation item has to be shown in the Global Navigation, optional and default to true.  

  

#### (optional) showInCurrentNavigation  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Defines whether the navigation item has to be shown in the Current Navigation, optional and default to true.  

  

### Return Value
Type: string  
The simple link URL just created.  


## See also
- [PageExtensions](Microsoft.SharePoint.Client.PageExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
