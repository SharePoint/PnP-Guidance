# NavigationExtensions.AddNavigationNode Method  
 Add a node to quick launch, top navigation bar or search navigation. The node will be added as the last node in the collection.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static NavigationNode AddNavigationNode(this Web web, String nodeTitle, Uri nodeUri, String parentNodeTitle, NavigationType navigationType, Boolean isExternal = False, Boolean asLastNode = True)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### nodeTitle  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;the title of node to add  

  

#### nodeUri  
&emsp;&emsp;Type: System.Uri  
&emsp;&emsp;the url of node to add  

  

#### parentNodeTitle  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;if string.Empty, then will add this node as top level node  

  

#### navigationType  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Enums.NavigationType](OfficeDevPnP.Core.Enums.NavigationType.md)  
&emsp;&emsp;the type of navigation, quick launch, top navigation or search navigation  

  

#### (optional) isExternal  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;true if the link is an external link  

  

#### (optional) asLastNode  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;true if the link should be added as the last node of the collection  

  

### Return Value
Type: NavigationNode  
Newly added NavigationNode  


## See also
- [NavigationExtensions](Microsoft.SharePoint.Client.NavigationExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
