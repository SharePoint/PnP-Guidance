# ExternalSharingExtensions.ShareSite Method  
 Share site for a person using just email. Will resolve needed people picker JSON value automatically.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static SharingResult ShareSite(this Web web, String email, ExternalSharingSiteOption shareOption, Boolean sendEmail = True, String emailBody = "Site shared for you.", Boolean useSimplifiedRoles = True)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web for the context of the site to be shared.  

  

#### email  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Email of the person to whom site should be shared.  

  

#### shareOption  
&emsp;&emsp;Type: [Microsoft.SharePoint.Client.ExternalSharingSiteOption](Microsoft.SharePoint.Client.ExternalSharingSiteOption.md)  
&emsp;&emsp;Sharing style - View, Edit, Owner  

  

#### (optional) sendEmail  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Should we send email for the given address.  

  

#### (optional) emailBody  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Text to be added on share email sent to receiver.  

  

#### (optional) useSimplifiedRoles  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Boolean value indicating whether to use the SharePoint simplified roles (Edit, View)  

  

### Return Value
Type: SharingResult  
A SharingResult object  


## See also
- [ExternalSharingExtensions](Microsoft.SharePoint.Client.ExternalSharingExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
