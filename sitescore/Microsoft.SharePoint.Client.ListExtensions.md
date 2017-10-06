# ListExtensions Class
 Class that holds deprecated generic list creation and manipulation methods 

 Class that provides generic list creation and manipulation methods   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class ListExtensions
```
## Extension Methods
|**Name**|**Description**|
|:-----|:-----|
| [AddRemoteEventReceiver(List, String, String, EventReceiverType, EventReceiverSynchronization, Boolean)](Microsoft.SharePoint.Client.ListExtensions.b9c036ed.md) | Registers a remote event receiver
| [AddRemoteEventReceiver(List, String, String, EventReceiverType, EventReceiverSynchronization, Int32, Boolean)](Microsoft.SharePoint.Client.ListExtensions.f19fbc38.md) | Registers a remote event receiver
| [AddWebhookSubscription(List, String, DateTime, String, String)](Microsoft.SharePoint.Client.ListExtensions.562ded14.md) | Add the a Webhook subscription to a list Note: If the access token is not specified, it will cost a dummy request to retrieve it
| [AddWebhookSubscription(List, String, Int32, String, String)](Microsoft.SharePoint.Client.ListExtensions.94d285b1.md) | Add the a Webhook subscription to a list Note: If the access token is not specified, it will cost a dummy request to retrieve it
| [CreateDocumentLibrary(Web, String, Boolean, String)](Microsoft.SharePoint.Client.ListExtensions.e18b841c.md) | Adds a document library to a web. Execute Query is called during this implementation
| [CreateList(Web, ListTemplateType, String, Boolean, Boolean, String, Boolean)](Microsoft.SharePoint.Client.ListExtensions.8c2b1d97.md) | Adds a default list to a site
| [CreateList(Web, Guid, Int32, String, Boolean, Boolean, String, Boolean)](Microsoft.SharePoint.Client.ListExtensions.bc245822.md) | Adds a custom list to a site
| [CreateView(List, String, ViewType, String[], UInt32, Boolean, String, Boolean, Boolean)](Microsoft.SharePoint.Client.ListExtensions.1a961e12.md) | Create view to existing list
| [CreateViewsFromXML(Web, String, XmlDocument)](Microsoft.SharePoint.Client.ListExtensions.eaed2442.md) | Create list views based on xml structure loaded to memory
| [CreateViewsFromXML(List, XmlDocument)](Microsoft.SharePoint.Client.ListExtensions.8b3c7905.md) | Actual implementation of the view creation logic based on given xml
| [CreateViewsFromXMLFile(Web, String, String)](Microsoft.SharePoint.Client.ListExtensions.1bdf14c8.md) | Creates list views based on specific xml structure from file
| [CreateViewsFromXMLFile(List, String)](Microsoft.SharePoint.Client.ListExtensions.7dfceb65.md) | Create list views based on specific xml structure in external file
| [CreateViewsFromXMLString(Web, String, String)](Microsoft.SharePoint.Client.ListExtensions.a682431e.md) | Creates views based on specific xml structure from string
| [CreateViewsFromXMLString(List, String)](Microsoft.SharePoint.Client.ListExtensions.e6e048f7.md) | Create list views based on specific xml structure in string
| [GetDefaultColumnValues(List)](Microsoft.SharePoint.Client.ListExtensions.b3d11314.md) | Gets default values for column values.The returned list contains one dictionary per default setting per folder.Each dictionary has the following keys set: Path, Field, ValuePath: Relative path to the library/folderField: Internal name of the field which has a default valueValue: The default value for the field
| [GetEventReceiverById(List, Guid)](Microsoft.SharePoint.Client.ListExtensions.63be7c1a.md) | Returns an event receiver definition
| [GetEventReceiverByName(List, String)](Microsoft.SharePoint.Client.ListExtensions.fcdeff9f.md) | Returns an event receiver definition
| [GetListByTitle(Web, String, Expression&lt;Func&lt;List, Object&gt;&gt;[])](Microsoft.SharePoint.Client.ListExtensions.8078cf54.md) | Get list by using Title
| [GetListByUrl(Web, String, Expression&lt;Func&lt;List, Object&gt;&gt;[])](Microsoft.SharePoint.Client.ListExtensions.45b98e2a.md) | Get list by using Url
| [GetListID(Web, String)](Microsoft.SharePoint.Client.ListExtensions.7e803d44.md) | Returns the GUID id of a list
| [GetPagesLibrary(Web)](Microsoft.SharePoint.Client.ListExtensions.72bc72eb.md) | Gets the publishing pages library of the web based on site language
| [GetPropertyBagValueInt(List, String, Int32)](Microsoft.SharePoint.Client.ListExtensions.1e690ec1.md) | Get int typed property bag value. If does not contain, returns default value.
| [GetPropertyBagValueString(List, String, String)](Microsoft.SharePoint.Client.ListExtensions.6838ef8b.md) | Get string typed property bag value. If does not contain, returns given default value.
| [GetViewById(List, Guid, Expression&lt;Func&lt;View, Object&gt;&gt;[])](Microsoft.SharePoint.Client.ListExtensions.77ca9349.md) | Gets a view by Id
| [GetViewByName(List, String, Expression&lt;Func&lt;View, Object&gt;&gt;[])](Microsoft.SharePoint.Client.ListExtensions.53d0489.md) | Gets a view by Name
| [GetWebhookSubscriptions(List, String)](Microsoft.SharePoint.Client.ListExtensions.15edb0e7.md) | Get all the existing Webhooks subscriptions of the list Note: If the access token is not specified, it will cost a dummy request to retrieve it
| [GetWebhookSubscriptionsAsync(List, String)](Microsoft.SharePoint.Client.ListExtensions.73f6d642.md) | Async get all the existing Webhooks subscriptions of the list Note: If the access token is not specified, it will cost a dummy request to retrieve it
| [GetWebRelativeUrl(List)](Microsoft.SharePoint.Client.ListExtensions.1d0b225d.md) | Gets the web relative URL. Allow users to get the web relative URL of a list. This is useful when exporting lists as it can then be used as a parameter to Web.GetListByUrl().
| [ListExists(Web, String)](Microsoft.SharePoint.Client.ListExtensions.696f8225.md) | Checks if list exists on the particular site based on the list Title property.
| [ListExists(Web, Uri)](Microsoft.SharePoint.Client.ListExtensions.18ffaeae.md) | Checks if list exists on the particular site based on the list's site relative path.
| [ListExists(Web, Guid)](Microsoft.SharePoint.Client.ListExtensions.b0dd134e.md) | Checks if list exists on the particular site based on the list id property.
| [PropertyBagContainsKey(List, String)](Microsoft.SharePoint.Client.ListExtensions.1fcb2c8b.md) | Checks if the given property bag entry exists
| [ReIndexList(List)](Microsoft.SharePoint.Client.ListExtensions.9d2ca161.md) | Queues a list for a full crawl the next incremental crawl
| [RemoveContentTypeByName(List, String)](Microsoft.SharePoint.Client.ListExtensions.8e0c93ca.md) | Removes a content type from a list/library by name
| [RemoveWebhookSubscription(List, String, String)](Microsoft.SharePoint.Client.ListExtensions.e742f4.md) | Remove a Webhook subscription from the list Note: If the access token is not specified, it will cost a dummy request to retrieve it
| [RemoveWebhookSubscription(List, Guid, String)](Microsoft.SharePoint.Client.ListExtensions.bafc4d30.md) | Remove a Webhook subscription from the list Note: If the access token is not specified, it will cost a dummy request to retrieve it
| [RemoveWebhookSubscription(List, WebhookSubscription, String)](Microsoft.SharePoint.Client.ListExtensions.12620e16.md) | Remove a Webhook subscription from the list Note: If the access token is not specified, it will cost a dummy request to retrieve it
| [SetDefaultColumnValues(List, IEnumerable&lt;IDefaultColumnValue&gt;)](Microsoft.SharePoint.Client.ListExtensions.4bb08d61.md) | Sets default values for column values.In order to for instance set the default Enterprise Metadata keyword field to a term, add the enterprise metadata keyword to a library (internal name "TaxKeyword")Column values are defined by the DefaultColumnValue class that has 3 properties:RelativeFolderPath : / to set a default value for the root of the document library, or /foldername to specify a subfolderFieldInternalName : The name of the field to set. For instance "TaxKeyword" to set the Enterprise Metadata fieldTerms : A collection of Taxonomy terms to setSupported column types: Metadata, Text, Choice, MultiChoice, People, Boolean, DateTime, Number, Currency
| [SetJSLinkCustomizations(List, PageType, String)](Microsoft.SharePoint.Client.ListExtensions.2f8c0ee3.md) | Sets JS link customization for a list form
| [SetJSLinkCustomizations(List, String, String)](Microsoft.SharePoint.Client.ListExtensions.81a6f21d.md) | Sets JS link customization for a list view page
| [SetListPermission(List, BuiltInIdentity, RoleType)](Microsoft.SharePoint.Client.ListExtensions.1f730c53.md) | Set custom permission to the list
| [SetListPermission(List, Principal, RoleType)](Microsoft.SharePoint.Client.ListExtensions.bd1961ba.md) | Set custom permission to the list
| [SetLocalizationLabelsForList(Web, String, String, String, String)](Microsoft.SharePoint.Client.ListExtensions.80380769.md) |  Can be used to set translations for different cultures. 
| [SetLocalizationLabelsForList(List, String, String, String)](Microsoft.SharePoint.Client.ListExtensions.8ed7fd4c.md) | Can be used to set translations for different cultures.
| [SetPropertyBagValue(List, String, Int32)](Microsoft.SharePoint.Client.ListExtensions.c741671e.md) | Sets a key/value pair in the web property bag
| [SetPropertyBagValue(List, String, String)](Microsoft.SharePoint.Client.ListExtensions.f4a64b4f.md) | Sets a key/value pair in the list property bag
| [UpdateListVersioning(Web, String, Boolean, Boolean, Boolean)](Microsoft.SharePoint.Client.ListExtensions.3db99d1b.md) | Enable/disable versioning on a list
| [UpdateListVersioning(List, Boolean, Boolean, Boolean)](Microsoft.SharePoint.Client.ListExtensions.9a7ebb3c.md) | Enable/disable versioning on a list
| [UpdateTaxonomyFieldDefaultValue(Web, String, String, String, Guid, Guid)](Microsoft.SharePoint.Client.ListExtensions.24c445b5.md) | Sets the default value for a managed metadata column in the specified list. This operation will not change existing items in the list
| [UpdateWebhookSubscription(List, String, String, DateTime, String)](Microsoft.SharePoint.Client.ListExtensions.42b0ceaa.md) | Updates a Webhook subscription from the list Note: If the access token is not specified, it will cost a dummy request to retrieve it
| [UpdateWebhookSubscription(List, Guid, String, DateTime, String)](Microsoft.SharePoint.Client.ListExtensions.c7f782d.md) | Updates a Webhook subscription from the list Note: If the access token is not specified, it will cost a dummy request to retrieve it
| [UpdateWebhookSubscription(List, WebhookSubscription, String)](Microsoft.SharePoint.Client.ListExtensions.90f7bd07.md) | Updates a Webhook subscription from the list Note: If the access token is not specified, it will cost a dummy request to retrieve it
## Examples
```C#
list.SetLocalizationForSiteLabels("fi-fi", "Name of the site in Finnish", "Description in Finnish");
            
```

## See also
- System.ArgumentException
- System.ArgumentNullException
- System.InvalidOperationException
- [http://blogs.msdn.com/b/vesku/archive/2014/03/20/office365-multilingual-content-types-site-columns-and-site-other-elements.aspx](http://blogs.msdn.com/b/vesku/archive/2014/03/20/office365-multilingual-content-types-site-columns-and-site-other-elements.aspx)
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)
