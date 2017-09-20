# ExternalSharingExtensions.GetObjectSharingSettingsForDocument Method  
 Get current sharing settings for document and load list of users it has been shared automatically.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static ObjectSharingSettings GetObjectSharingSettingsForDocument(this Web web, String urlToDocument, Boolean useSimplifiedPolicies = True)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web for the context  

  

#### urlToDocument  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Full URL to the file which is shared  

  

#### (optional) useSimplifiedPolicies  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Boolean value indicating whether to use the SharePoint simplified roles (Edit, View).  

  

### Return Value
Type: ObjectSharingSettings  
A ObjectSharingSettings object  


## See also
- [ExternalSharingExtensions](Microsoft.SharePoint.Client.ExternalSharingExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
