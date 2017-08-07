# IRMSettings Class
 Declares the Information Rights Management settings for the list or library.   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel](OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel.md)  
## Syntax
```C#
public class IRMSettings: BaseModel, IEquatable<IRMSettings>
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [IRMSettings()](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.ctor1.md) |  Declares the Information Rights Management settings for the list or library. 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [AllowPrint](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.AllowPrint.md) | Defines whether a viewer can print the downloaded document.
| [AllowScript](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.AllowScript.md) | Defines whether a viewer can run a script on the downloaded document.
| [AllowWriteCopy](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.AllowWriteCopy.md) | Defines whether a viewer can write on a copy of the downloaded document.
| [DisableDocumentBrowserView](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.DisableDocumentBrowserView.md) | Defines whether to block Office Web Application Companion applications (WACs) from showing this document.
| [DocumentAccessExpireDays](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.DocumentAccessExpireDays.md) | Defines the number of days after which the downloaded document will expire.
| [DocumentLibraryProtectionExpiresInDays](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.DocumentLibraryProtectionExpiresInDays.md) | Defines the expire days for the Information Rights Management (IRM) protection of this document library will expire.
| [Enabled](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.Enabled.md) | Defines whether the IRM settings have to be enabled or not.
| [EnableDocumentAccessExpire](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.EnableDocumentAccessExpire.md) | Defines whether the downloaded document will expire.
| [EnableDocumentBrowserPublishingView](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.EnableDocumentBrowserPublishingView.md) | Defines whether to enable Office Web Application Companion applications (WACs) to publishing view.
| [EnableGroupProtection](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.EnableGroupProtection.md) | Defines whether the permission of the downloaded document is applicable to a group.
| [EnableLicenseCacheExpire](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.EnableLicenseCacheExpire.md) | Defines whether a user must verify their credentials after some interval.
| [GroupName](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.GroupName.md) | Defines the group name (email address) that the permission is also applicable to.
| [LicenseCacheExpireDays](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.LicenseCacheExpireDays.md) | Defines the number of days that the application that opens the document caches the IRM license. When these elapse, the application will connect to the IRM server to validate the license.
| [PolicyDescription](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.PolicyDescription.md) | Defines the permission policy description.
| [PolicyTitle](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.PolicyTitle.md) | Defines the permission policy title.
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Equals(Object)](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.3520ddbb.md) | Compares object with ObjectSecurity
| [Equals(IRMSettings)](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.ee183aec.md) | Compares IRMSettings object based on Enabled, AllowPrint, AllowScript, AllowWriteCopy, DisableDocumentBrowserView, DocumentAccessExpireDays, DocumentLibraryProtectionExpiresInDays, EnableDocumentAccessExpire, EnableDocumentBrowserPublishingView, EnableGroupProtection, EnableLicenseCacheExpire, GroupName, LicenseCacheExpireDays, PolicyDescription, and PolicyTitle
| [GetHashCode()](OfficeDevPnP.Core.Framework.Provisioning.Model.IRMSettings.1c6872bd.md) | Gets the hash code
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
