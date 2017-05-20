# ListExtensions.SetJSLinkCustomizations Method  
 Sets JS link customization for a list view page   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetJSLinkCustomizations(this List list, String serverRelativeUrl, String jslink)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;SharePoint list  

  

#### serverRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;url of the view page  

  

#### jslink  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;JSLink to set to the form. Set to empty string to remove the set JSLink customization. Specify multiple values separated by pipe symbol. For e.g.: ~sitecollection/_catalogs/masterpage/jquery-2.1.0.min.js|~sitecollection/_catalogs/masterpage/custom.js   

  

### Return Value
Type: void  

## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
