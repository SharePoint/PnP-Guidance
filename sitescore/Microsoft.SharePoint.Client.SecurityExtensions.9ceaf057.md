# SecurityExtensions.AssociateDefaultGroups Method  
 Associate the provided groups as default owners, members or visitors groups. If a group is null then the association is not done   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void AssociateDefaultGroups(this Web web, Group owners, Group members, Group visitors)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to operate on  

  

#### owners  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Group  
&emsp;&emsp;Owners group  

  

#### members  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Group  
&emsp;&emsp;Members group  

  

#### visitors  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Group  
&emsp;&emsp;Visitors group  

  

### Return Value
Type: void  

## See also
- [SecurityExtensions](Microsoft.SharePoint.Client.SecurityExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
