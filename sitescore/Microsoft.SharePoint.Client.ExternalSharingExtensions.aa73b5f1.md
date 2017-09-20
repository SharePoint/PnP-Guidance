# ExternalSharingExtensions.InviteExternalUser Method  
 Invites an external user as a group member   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static SharingResult InviteExternalUser(this Group group, String email, Boolean sendEmail = True, String emailBody = "Site shared with you.")
```
### Parameters
#### group  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Group  
&emsp;&emsp;Group to add the user to  

  

#### email  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The email address of the external user  

  

#### (optional) sendEmail  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Should we send an email to the given address  

  

#### (optional) emailBody  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Text to be added to the email  

  

### Return Value
Type: SharingResult  
A SharingResult object  


## See also
- [ExternalSharingExtensions](Microsoft.SharePoint.Client.ExternalSharingExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
