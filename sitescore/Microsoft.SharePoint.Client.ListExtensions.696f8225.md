# ListExtensions.ListExists Method  
 Checks if list exists on the particular site based on the list Title property.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool ListExists(this Web web, String listTitle)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### listTitle  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Title of the list to be checked.  

  

### Return Value
Type: bool  
True if the list exists  


## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- System.ArgumentException
- System.ArgumentNullException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
