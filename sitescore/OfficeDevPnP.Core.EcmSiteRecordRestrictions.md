# EcmSiteRecordRestrictions  enumeration
Specify restrictions to place on a document or item once it has been declared as a record. Changing this setting will not affect items which have already been declared records.  

**Namespace:** [OfficeDevPnP.Core](OfficeDevPnP.Core.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public enum EcmSiteRecordRestrictions
```
## Members
|**Member Name**|**Description**|
|:-----|:-----|
| Unknown | 
| None | Records are no more restricted than non-records
| BlockDelete | Records can be edited but not deleted
| BlockEdit | Records cannot be edited or deleted. Any change will require the record declaration to be revoked

## See also
- [OfficeDevPnP.Core](OfficeDevPnP.Core.md)
