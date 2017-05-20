# ExternalSharingExtensions.ShareDocument Method  
 Abstracted methid for sharing documents just with given email address.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static SharingResult ShareDocument(this Web web, String urlToDocument, String targetEmailToShare, ExternalSharingDocumentOption shareOption, Boolean sendEmail = True, String emailBody = "Document shared", Boolean useSimplifiedRoles = True)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web for the context used for people picker search  

  

#### urlToDocument  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Full URL to the file which is shared  

  

#### targetEmailToShare  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Email address for the person to whom the document will be shared  

  

#### shareOption  
&emsp;&emsp;Type: [Microsoft.SharePoint.Client.ExternalSharingDocumentOption](Microsoft.SharePoint.Client.ExternalSharingDocumentOption.md)  
&emsp;&emsp;View or Edit option  

  

#### (optional) sendEmail  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Send email or not  

  

#### (optional) emailBody  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Text attached to the email sent for the person to whom the document is shared  

  

#### (optional) useSimplifiedRoles  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Boolean value indicating whether to use the SharePoint simplified roles (Edit, View)  

  

### Return Value
Type: SharingResult  

## See also
- [ExternalSharingExtensions](Microsoft.SharePoint.Client.ExternalSharingExtensions.md) 
- [Microsoft.SharePoint.Client.ExternalSharingExtensions.ShareDocument(Microsoft.SharePoint.Client.Web,System.String,System.String,Microsoft.SharePoint.Client.ExternalSharingDocumentOption,System.Boolean,System.String,System.Boolean)](Microsoft.SharePoint.Client.ExternalSharingExtensions.66dc7567.md)
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
