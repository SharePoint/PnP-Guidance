# ListExtensions.GetListID Method  
 Returns the GUID id of a list   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Guid GetListID(this Web web, String listName)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### listName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;List to operate on  

  

### Return Value
Type: Guid  

## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- System.ArgumentException
- System.ArgumentNullException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
