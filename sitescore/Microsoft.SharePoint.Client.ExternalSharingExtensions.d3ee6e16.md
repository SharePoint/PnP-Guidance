# ExternalSharingExtensions.ShareSiteWithPeoplePickerValue Method  
 Share site for a person using complex JSON object for people picker value.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static SharingResult ShareSiteWithPeoplePickerValue(Web web, String peoplePickerInput, Group group, Boolean sendEmail, String emailBody)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Web for the context of the site to be shared.  

  

#### peoplePickerInput  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;JSON object with the people picker value  

  

#### group  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Group  
&emsp;&emsp;The group to invite the user to  

  

#### (optional) sendEmail  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Should we send email for the given address.  

  

#### (optional) emailBody  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Text to be added on share email sent to receiver.  

  

### Return Value
Type: SharingResult  
  


## Remarks
  
## See also
- [ExternalSharingExtensions](Microsoft.SharePoint.Client.ExternalSharingExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
