# FieldAndContentTypeExtensions Class
 This class holds deprecated extension methods that will help you work with fields and content types. 

 This class provides extension methods that will help you work with fields and content types.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class FieldAndContentTypeExtensions
```
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [FormatFieldXml(FieldCreationInformation)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.f06bc135.md) | Formats a fieldcreationinformation object into Field CAML xml.
## Extension Methods
|**Name**|**Description**|
|:-----|:-----|
| [AddContentTypeToList(Web, String, ContentType, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.8015fdd1.md) | Adds content type to list
| [AddContentTypeToList(List, ContentType, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.7070361c.md) | Add content type to list
| [AddContentTypeToListById(Web, String, String, Boolean, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.55771f16.md) | Adds content type to list
| [AddContentTypeToListById(List, String, Boolean, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.d2e9cbaa.md) | Add content type to list
| [AddContentTypeToListByName(Web, String, String, Boolean, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.4bee1f7d.md) | Adds content type to list
| [AddContentTypeToListByName(List, String, Boolean, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.5194e73a.md) | Add content type to list
| [AddFieldById(ContentType, String, Boolean, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.b2913ba1.md) | Associates field to content type
| [AddFieldById(ContentType, Guid, Boolean, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.8cc9483e.md) | Associates field to content type
| [AddFieldByName(ContentType, String, Boolean, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.7439ef2.md) | Associates field to content type
| [AddFieldToContentType(Web, ContentType, Field, Boolean, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.3d349624.md) | Associates field to content type
| [AddFieldToContentTypeById(Web, String, String, Boolean, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.960a9456.md) | Associates field to content type
| [AddFieldToContentTypeByName(Web, String, Guid, Boolean, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.539b980f.md) | Associates field to content type
| [BestMatch(ContentTypeCollection, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.e1d069b0.md) | Searches for the content type with the closest match to the value of the specified content type ID. If the search finds two matches, the shorter ID is returned.
| [BestMatchContentTypeId(List, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.eab7e452.md) | Searches the list content types and returns the content type identifier (ID) that is the nearest match to the specified content type ID.
| [ContentTypeExistsById(Web, String, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.5ef3bfd6.md) | Does content type exists in the web
| [ContentTypeExistsById(Web, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.a050753e.md) | Does content type exist in web
| [ContentTypeExistsById(List, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.12bea999.md) | Does content type exist in list
| [ContentTypeExistsByName(Web, String, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.3b90d49f.md) | Does content type exists in the web
| [ContentTypeExistsByName(Web, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.bbda9d79.md) | Does content type exist in web
| [ContentTypeExistsByName(List, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.64884576.md) | Does content type exist in list
| [CreateContentType(Web, String, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.63c9d5bf.md) | Create new content type to web
| [CreateContentType(Web, String, String, String, String, ContentType)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.838928a.md) | Create new content type to web
| [CreateContentTypeFromXML(Web, XDocument)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.ccafd6b.md) | Create a content type based on the classic feature framework structure.
| [CreateContentTypeFromXMLFile(Web, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.521fec1b.md) | Create a content type based on the classic feature framework structure.
| [CreateContentTypeFromXMLString(Web, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.5df0e3e9.md) | Create a content type based on the classic feature framework structure.
| [CreateField(Web, FieldCreationInformation, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.c9f9b03f.md) | Create field to web remotely / Create field to web remotely
| [CreateField&lt;TField&gt;(Web, FieldCreationInformation, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.c9f9b03f.md) | 
| [CreateField(Web, String, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.8be6143a.md) | Create field to web remotely
| [CreateField(List, FieldCreationInformation, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.9167a54e.md) | Adds field to a list / Adds field to a list
| [CreateField&lt;TField&gt;(List, FieldCreationInformation, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.9167a54e.md) | 
| [CreateField(List, String, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.db895c0.md) | Adds a field to a list
| [CreateFieldsFromXML(Web, XDocument)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.9bc8d719.md) | Creates field from xml structure which follows the classic feature framework structure
| [CreateFieldsFromXMLFile(Web, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.c7cd2cf8.md) | Creates fields from feature element xml file schema. XML file can contain one or many field definitions created using classic feature framework structure.
| [CreateFieldsFromXMLString(Web, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.abeb1e95.md) | Creates fields from feature element xml file schema. XML file can contain one or many field definitions created using classic feature framework structure.
| [DeleteContentTypeById(Web, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.7db8c43a.md) | Deletes a content type from the web by id
| [DeleteContentTypeByName(Web, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.76b85598.md) | Deletes a content type from the web by name
| [FieldExistsById(Web, Guid, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.7b2d21bf.md) | Returns if the field is found
| [FieldExistsById(Web, String, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.d7fd74d3.md) | Does field exist in web
| [FieldExistsById(List, Guid)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.e6f3bec3.md) | Returns if the field is found
| [FieldExistsById(List, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.54a82652.md) | Returns if the field is found, query based on the ID
| [FieldExistsByName(Web, String, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.2d7862f8.md) | Returns if the field is found
| [FieldExistsByName(List, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.67ff82ce.md) | Field exists in list by name
| [FieldExistsByNameInContentType(Web, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.6b483df3.md) | Field exists in content type
| [FieldExistsByNameInContentType(ContentType, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.470ae95f.md) | Checks if a field exists in a content type by id
| [GetContentTypeById(Web, String, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.9e769121.md) | Return content type by Id
| [GetContentTypeById(List, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.5ba34f83.md) | Return content type by Id
| [GetContentTypeByName(Web, String, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.dac8c10a.md) | Return content type by name
| [GetContentTypeByName(List, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.7e65e981.md) | Return content type by name
| [GetFieldById&lt;TField&gt;(Web, Guid, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.a552175c.md) | Returns the field if it exists. Null if it does not exist. / Returns the field if it exists. Null if it does not exist.
| [GetFieldById(Web, Guid, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.a552175c.md) | 
| [GetFieldById&lt;TField&gt;(List, Guid)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.f00c000f.md) | Returns the field if it exists. Null if it does not exist. / Returns the field if it exists. Null if it does not exist.
| [GetFieldById(List, Guid)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.f00c000f.md) | 
| [GetFieldByInternalName(Web, String, Boolean)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.3ca86595.md) | Returns the field if it exists. Null if does not exist.
| [GetFieldByInternalName&lt;TField&gt;(FieldCollection, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.a6b12c6.md) | Returns the field if it exists. Null if it does not exist. / Returns the field if it exists. Null if it does not exist.
| [GetFieldByInternalName(FieldCollection, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.a6b12c6.md) | 
| [GetFieldByName&lt;TField&gt;(FieldCollection, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.db62d2bc.md) | Returns the field if it exists. Null if it does not exist. / Returns the field if it exists. Null if it does not exist.
| [GetFieldByName(FieldCollection, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.db62d2bc.md) | 
| [GetFields(List, String[])](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.96a2398f.md) | Gets a list of fields from a list by names.
| [RemoveContentTypeFromList(Web, List, ContentType)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.ed537a75.md) | Removes content type from a list
| [RemoveContentTypeFromListById(Web, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.8a877f1a.md) | Removes content type from a list
| [RemoveContentTypeFromListById(Web, List, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.88667cf4.md) | Removes content type from a list
| [RemoveContentTypeFromListByName(Web, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.8333f667.md) | Removes content type from list
| [RemoveContentTypeFromListByName(Web, List, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.8aac8612.md) | Removes content type from list
| [RemoveFieldById(Web, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.7f3bcd91.md) | Removes a field by specifying its ID
| [RemoveFieldByInternalName(Web, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.d0b69cca.md) | Removes a field by specifying its internal name
| [ReorderContentTypes(List, IEnumerable&lt;String&gt;)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.215c7c05.md) | Reorders content types on the list. The first one in the list is the default item. Any items left out from the list will still be on the content type, but will not be visible on the new button.
| [SetDefaultContentTypeToList(Web, List, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.6b5dce6c.md) | Set default content type to list
| [SetDefaultContentTypeToList(Web, List, ContentType)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.156c371a.md) | Set default content type to list
| [SetDefaultContentTypeToList(Web, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.43df7b04.md) | Set default content type to list
| [SetDefaultContentTypeToList(Web, String, ContentType)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.658dabc5.md) | Set's default content type list.
| [SetDefaultContentTypeToList(List, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.f809c93d.md) | Set's default content type list.
| [SetDefaultContentTypeToList(List, ContentType)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.deceb25a.md) | Set default content type to list
| [SetJsLinkCustomizations(Field, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.5f46c9a2.md) | Adds jsLink to a field.
| [SetJsLinkCustomizations(List, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.ac751d3.md) | Adds jsLink to a list field.
| [SetLocalizationForContentType(Web, String, String, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.c2130165.md) | Set localized labels for content type
| [SetLocalizationForContentType(List, String, String, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.4d67b41c.md) | Set localized labels for content type
| [SetLocalizationForContentType(ContentType, String, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.e7593abe.md) | Set localized labels for content type
| [SetLocalizationForField(Web, Guid, String, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.d0922668.md) | Set localized labels for field
| [SetLocalizationForField(Web, String, String, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.23c901fd.md) | Set localized labels for field
| [SetLocalizationForField(Web, Field, String, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.4786ffe9.md) | Set localized labels for field
| [SetLocalizationForField(List, Guid, String, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.422fb615.md) | Set localized labels for field
| [SetLocalizationForField(List, String, String, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.791c339c.md) | Set localized labels for field
| [SetLocalizationForField(List, Field, String, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.be84de34.md) | Set localized labels for field
| [SetLocalizationForField(Field, String, String, String)](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.2d7ccffd.md) | Set localized labels for field
## See also
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)
