# DocumentSetTemplate Class
 Defines a DocumentSet Template for creating multiple DocumentSet instances   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel](OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel.md)  
## Syntax
```C#
public class DocumentSetTemplate: BaseModel, IEquatable<DocumentSetTemplate>
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [DocumentSetTemplate()](OfficeDevPnP.Core.Framework.Provisioning.Model.DocumentSetTemplate.ctor1.md) | Constructor for DocumentSetTemplate class 
| [DocumentSetTemplate(String, IEnumerable<String>, IEnumerable<DefaultDocument>, IEnumerable<Guid>, IEnumerable<Guid>)](OfficeDevPnP.Core.Framework.Provisioning.Model.DocumentSetTemplate.ctor2.md) | Constructor for DocumentSetTemplate class 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [AllowedContentTypes](OfficeDevPnP.Core.Framework.Provisioning.Model.DocumentSetTemplate.AllowedContentTypes.md) | The list of allowed Content Types for the Document Set
| [DefaultDocuments](OfficeDevPnP.Core.Framework.Provisioning.Model.DocumentSetTemplate.DefaultDocuments.md) | The list of default Documents for the Document Set
| [RemoveExistingContentTypes](OfficeDevPnP.Core.Framework.Provisioning.Model.DocumentSetTemplate.RemoveExistingContentTypes.md) | The RemoveExistingContentTypes flag for the Allowed Content Types of the current Document Set, optional attribute.
| [SharedFields](OfficeDevPnP.Core.Framework.Provisioning.Model.DocumentSetTemplate.SharedFields.md) | The list of Shared Fields for the Document Set
| [WelcomePage](OfficeDevPnP.Core.Framework.Provisioning.Model.DocumentSetTemplate.WelcomePage.md) | Defines the custom WelcomePage for the Document Set
| [WelcomePageFields](OfficeDevPnP.Core.Framework.Provisioning.Model.DocumentSetTemplate.WelcomePageFields.md) | The list of Welcome Page Fields for the Document Set
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Equals(Object)](OfficeDevPnP.Core.Framework.Provisioning.Model.DocumentSetTemplate.3520ddbb.md) | Compares object with DocumentSetTemplate
| [Equals(DocumentSetTemplate)](OfficeDevPnP.Core.Framework.Provisioning.Model.DocumentSetTemplate.9b91d7be.md) | Compares DocumentSetTemplate object based on AllowedContentTypes, DefaultDocuments, SharedFields, WelcomePageFields, and RemoveExistingContentTypes properties.
| [GetHashCode()](OfficeDevPnP.Core.Framework.Provisioning.Model.DocumentSetTemplate.1c6872bd.md) | Gets the hash code
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
