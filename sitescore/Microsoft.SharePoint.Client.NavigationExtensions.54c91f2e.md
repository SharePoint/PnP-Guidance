# NavigationExtensions.DeleteNavigationNode Method  
 Deletes a navigation node from the quickLaunch or top navigation bar   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void DeleteNavigationNode(this Web web, String nodeTitle, String parentNodeTitle, NavigationType navigationType)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### nodeTitle  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;the title of node to delete  

  

#### parentNodeTitle  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;if string.Empty, then will delete this node as top level node  

  

#### navigationType  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Enums.NavigationType](OfficeDevPnP.Core.Enums.NavigationType.md)  
&emsp;&emsp;the type of navigation, quick launch, top navigation or search navigation  

  

### Return Value
Type: void  

## See also
- [NavigationExtensions](Microsoft.SharePoint.Client.NavigationExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
