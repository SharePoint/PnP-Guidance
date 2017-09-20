# ExternalSharingExtensions Class
 This class holds the methods for sharing and unsharing of the document and the site.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class ExternalSharingExtensions
```
## Extension Methods
|**Name**|**Description**|
|:-----|:-----|
| [CreateAnonymousLinkForDocument(Web, String, ExternalSharingDocumentOption)](Microsoft.SharePoint.Client.ExternalSharingExtensions.65ade625.md) |  Creates anonymous link to given document. See MSDN
| [CreateAnonymousLinkWithExpirationForDocument(Web, String, ExternalSharingDocumentOption, DateTime)](Microsoft.SharePoint.Client.ExternalSharingExtensions.d634f954.md) |  Creates anonymous link to the given document with automatic expiration time. See MSDN
| [GetObjectSharingSettingsForDocument(Web, String, Boolean)](Microsoft.SharePoint.Client.ExternalSharingExtensions.f6e910ee.md) | Get current sharing settings for document and load list of users it has been shared automatically.
| [GetObjectSharingSettingsForSite(Web, Boolean)](Microsoft.SharePoint.Client.ExternalSharingExtensions.67d0238b.md) | Get current sharing settings for site and load list of users it has been shared automatically.
| [InviteExternalUser(Group, String, Boolean, String)](Microsoft.SharePoint.Client.ExternalSharingExtensions.aa73b5f1.md) | Invites an external user as a group member
| [ResolvePeoplePickerValueForEmail(Web, String)](Microsoft.SharePoint.Client.ExternalSharingExtensions.7657a39c.md) |  Can be used to get needed people picker search result value for given email account. See MSDN
| [ShareDocument(Web, String, String, ExternalSharingDocumentOption, Boolean, String, Boolean)](Microsoft.SharePoint.Client.ExternalSharingExtensions.66dc7567.md) | Abstracted methid for sharing documents just with given email address.
| [ShareDocumentWithPeoplePickerValue(Web, String, String, ExternalSharingDocumentOption, Boolean, String, Boolean)](Microsoft.SharePoint.Client.ExternalSharingExtensions.1122069f.md) | Share document with complex JSON string value.
| [ShareSite(Web, String, Group, Boolean, String)](Microsoft.SharePoint.Client.ExternalSharingExtensions.3710fea1.md) | Share site for a person using just email. Will resolve needed people picker JSON value automatically.
| [ShareSite(Web, String, ExternalSharingSiteOption, Boolean, String, Boolean)](Microsoft.SharePoint.Client.ExternalSharingExtensions.e85402ce.md) | Share site for a person using just email. Will resolve needed people picker JSON value automatically.
| [ShareSiteWithPeoplePickerValue(Web, String, ExternalSharingSiteOption, Boolean, String, Boolean)](Microsoft.SharePoint.Client.ExternalSharingExtensions.7e4b4d30.md) | Share site for a person using complex JSON object for people picker value.
| [ShareSiteWithPeoplePickerValue(Web, String, Group, Boolean, String)](Microsoft.SharePoint.Client.ExternalSharingExtensions.d3ee6e16.md) | Share site for a person using complex JSON object for people picker value.
| [UnshareDocument(Web, String)](Microsoft.SharePoint.Client.ExternalSharingExtensions.fa304889.md) | Can be used to programatically to unshare any document with the document URL.
## See also
- Microsoft.SharePoint.Client.ExternalSharingExtensions.ShareDocument(Microsoft.SharePoint.Client.Web,System.String,System.String,Microsoft.SharePoint.Client.ExternalSharingDocumentOption,System.Boolean,System.String,System.Boolean)
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)
