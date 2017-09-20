# ListExtensions.SetListPermission Method  
 Set custom permission to the list   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetListPermission(this List list, BuiltInIdentity user, RoleType roleType)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;List on which permission to be set  

  

#### user  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Enums.BuiltInIdentity](OfficeDevPnP.Core.Enums.BuiltInIdentity.md)  
&emsp;&emsp;Built in user  

  

#### roleType  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.RoleType  
&emsp;&emsp;Role type  

  

### Return Value
Type: void  

## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
