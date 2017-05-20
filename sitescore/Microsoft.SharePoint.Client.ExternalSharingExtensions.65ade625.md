# ExternalSharingExtensions.CreateAnonymousLinkForDocument Method  
 Creates anonymous link to given document. See MSDN  

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static string CreateAnonymousLinkForDocument(this Web web, String urlToDocument, ExternalSharingDocumentOption shareOption)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web for the context used for people picker search  

  

#### urlToDocument  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Full URL to the file which is shared  

  

#### shareOption  
&emsp;&emsp;Type: [Microsoft.SharePoint.Client.ExternalSharingDocumentOption](Microsoft.SharePoint.Client.ExternalSharingDocumentOption.md)  
&emsp;&emsp;Type of the link to be created - View or Edit  

  

### Return Value
Type: string  
Anonymous URL to the file as string  


## See also
- [ExternalSharingExtensions](Microsoft.SharePoint.Client.ExternalSharingExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
