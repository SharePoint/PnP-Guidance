# RecordsManagementExtensions Class
 Class that deals with deprecated records management functionality 

 Class that deals with records management functionality   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class RecordsManagementExtensions
```
## Extension Methods
|**Name**|**Description**|
|:-----|:-----|
| [ActivateInPlaceRecordsManagementFeature(Site)](Microsoft.SharePoint.Client.RecordsManagementExtensions.3537381f.md) | Activate the in place records management feature
| [DisableInPlaceRecordsManagementFeature(Site)](Microsoft.SharePoint.Client.RecordsManagementExtensions.8c9a2d70.md) | Deactivate the in place records management feature
| [EnableSiteForInPlaceRecordsManagement(Site)](Microsoft.SharePoint.Client.RecordsManagementExtensions.1993740d.md) | Enable in place records management. The in place records management feature will be enabled and the in place record management will be enabled in all locations with record declaration allowed by all contributors and undeclaration by site admins
| [GetListAutoRecordDeclaration(List)](Microsoft.SharePoint.Client.RecordsManagementExtensions.c12e805c.md) | Returns if auto record declaration is active for this list
| [GetListManualRecordDeclaration(List)](Microsoft.SharePoint.Client.RecordsManagementExtensions.b115669f.md) | Gets the manual in place record declaration for this list
| [GetManualRecordDeclarationInAllLocations(Site)](Microsoft.SharePoint.Client.RecordsManagementExtensions.63e928bb.md) | Get the value of the records management is allowed in all places setting
| [GetRecordDeclarationBy(Site)](Microsoft.SharePoint.Client.RecordsManagementExtensions.8a882c7d.md) | Gets who can declare records
| [GetRecordRestrictions(Site)](Microsoft.SharePoint.Client.RecordsManagementExtensions.5d44e2d3.md) | Gets the current restrictions on declared records
| [GetRecordUnDeclarationBy(Site)](Microsoft.SharePoint.Client.RecordsManagementExtensions.526b1349.md) | Gets who can undeclare records
| [IsInPlaceRecordsManagementActive(Site)](Microsoft.SharePoint.Client.RecordsManagementExtensions.43c6a592.md) | Checks if in place records management functionality is enabled for this site collection
| [IsListRecordSettingDefined(List)](Microsoft.SharePoint.Client.RecordsManagementExtensions.de1b84fc.md) | Checks if this list has active in place records management settings defined
| [SetListAutoRecordDeclaration(List, Boolean)](Microsoft.SharePoint.Client.RecordsManagementExtensions.b8e7f815.md) | Defines if auto record declaration is active for this list: all added items will be automatically declared as a record if active
| [SetListManualRecordDeclaration(List, EcmListManualRecordDeclaration)](Microsoft.SharePoint.Client.RecordsManagementExtensions.9a469feb.md) | Defines the manual in place record declaration for this list
| [SetManualRecordDeclarationInAllLocations(Site, Boolean)](Microsoft.SharePoint.Client.RecordsManagementExtensions.e5a750b4.md) | Defines if in place records management is allowed in all places
| [SetRecordDeclarationBy(Site, EcmRecordDeclarationBy)](Microsoft.SharePoint.Client.RecordsManagementExtensions.47914e62.md) | Defines who can declare records
| [SetRecordRestrictions(Site, EcmSiteRecordRestrictions)](Microsoft.SharePoint.Client.RecordsManagementExtensions.1b685f24.md) | Defines the restrictions that are placed on a document once it's declared as a record
| [SetRecordUnDeclarationBy(Site, EcmRecordDeclarationBy)](Microsoft.SharePoint.Client.RecordsManagementExtensions.794eadc1.md) | Defines who can undeclare records
## See also
- [OfficeDevPnP.Core.EcmListManualRecordDeclaration](OfficeDevPnP.Core.EcmListManualRecordDeclaration.md)
- [OfficeDevPnP.Core.EcmRecordDeclarationBy](OfficeDevPnP.Core.EcmRecordDeclarationBy.md)
- [OfficeDevPnP.Core.EcmSiteRecordRestrictions](OfficeDevPnP.Core.EcmSiteRecordRestrictions.md)
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)
