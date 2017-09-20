# SecurityExtensions.AddReaderAccess Method  
 Add read access to the group "Everyone except external users".   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static User AddReaderAccess(this Web web, BuiltInIdentity user)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### user  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Enums.BuiltInIdentity](OfficeDevPnP.Core.Enums.BuiltInIdentity.md)  
&emsp;&emsp;Built in user to add to the visitors group  

  

### Return Value
Type: User  

## See also
- [SecurityExtensions](Microsoft.SharePoint.Client.SecurityExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
