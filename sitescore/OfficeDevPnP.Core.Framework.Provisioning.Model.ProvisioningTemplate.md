# ProvisioningTemplate Class
 Domain Object for the Provisioning Template 

 Domain Object for the Provisioning Template   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public class ProvisioningTemplate: IEquatable<ProvisioningTemplate>
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [ProvisioningTemplate()](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.ctor1.md) | Constructor for ProvisioningTemplate class 
| [ProvisioningTemplate(FileConnectorBase)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.ctor2.md) | Constructor for ProvisioningTemplate class 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [AddIns](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.AddIns.md) | Defines the SharePoint Add-ins to provision
| [AuditSettings](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.AuditSettings.md) | The Audit Settings for the Provisioning Template
| [BaseSiteTemplate](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.BaseSiteTemplate.md) | The Base SiteTemplate of the Provisioning Template
| [ClientSidePages](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.ClientSidePages.md) | Gets a collection of ClientSidePage to configure for the site
| [ComposedLook](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.ComposedLook.md) | Gets or Sets the composed look of the template
| [Connector](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Connector.md) | Gets or sets the File Connector
| [ContentTypes](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.ContentTypes.md) | Gets a collection of Content Types to create
| [CustomActions](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.CustomActions.md) | Gets or sets CustomActions for the template
| [Description](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Description.md) | The Description of the Provisioning Template
| [Directories](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Directories.md) | Gets a collection of directories from which upload files for the template
| [DisplayName](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.DisplayName.md) | The Display Name of the Provisioning Template
| [ExtensibilityHandlers](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.ExtensibilityHandlers.md) | Gets or sets the Extensibility Handlers
| [Features](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Features.md) | Gets or sets a list of features to activate or deactivate
| [Files](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Files.md) | Gets a collection of files for the template
| [Id](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Id.md) | Gets or sets the ID of the Provisioning Template
| [ImagePreviewUrl](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.ImagePreviewUrl.md) | The Image Preview Url of the Provisioning Template
| [Lists](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Lists.md) | 
| [Localizations](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Localizations.md) | Gets or sets the Localizations
| [Navigation](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Navigation.md) | The Navigation configurations of the Provisioning Template
| [Pages](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Pages.md) | Gets a collection of Wiki Pages for the template
| [Parameters](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Parameters.md) | Any parameters that can be used throughout the template
| [Properties](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Properties.md) | A set of custom Properties for the Provisioning Template
| [PropertyBagEntries](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.PropertyBagEntries.md) | 
| [Providers](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Providers.md) | Gets a collection of Providers that are used during the extensibility pipeline
| [Publishing](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Publishing.md) | Defines the Publishing configuration to provision
| [RegionalSettings](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.RegionalSettings.md) | The Regional Settings of the Provisioning Template
| [Scope](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Scope.md) | Declares the target scope of the current Provisioning Template
| [SearchSettings](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.SearchSettings.md) | The Search Settings for the Provisioning Template
| [Security](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Security.md) | Security Groups Members for the Template
| [SiteFields](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.SiteFields.md) | Gets a collection of fields
| [SitePolicy](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.SitePolicy.md) | Gets or Sets the Site Policy
| [SiteSearchSettings](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.SiteSearchSettings.md) | The Site Collection level Search Settings for the Provisioning Template
| [SiteWebhooks](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.SiteWebhooks.md) | Gets a collection of SiteWebhooks to configure for the site
| [SupportedUILanguages](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.SupportedUILanguages.md) | The Supported UI Languages for the Provisioning Template
| [TemplateCultureInfo](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.TemplateCultureInfo.md) | The default CultureInfo of the Provisioning Template, used to format all input values, optional attribute.
| [TermGroups](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.TermGroups.md) | Gets a collection of termgroups to deploy to the site
| [Version](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Version.md) | Gets or sets the Version of the Provisioning Template
| [WebSearchSettings](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.WebSearchSettings.md) | The Web level Search Settings for the Provisioning Template
| [WebSettings](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.WebSettings.md) | The Web Settings of the Provisioning Template
| [Workflows](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.Workflows.md) | Defines the Workflows to provision
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Equals(Object)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.3520ddbb.md) | Compares object with ProvisioningTemplate
| [Equals(ProvisioningTemplate)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.89c2b310.md) | Compares ProvisioningTemplate object based on ComposedLook, ContentTypes, CustomActions, SiteFeature, WebFeatures, Files, Id, Lists, PropertyBagEntries, Providers, Security, SiteFields, SitePolicy, Version, Pages, TermGroups, Workflows, AddIns, Publishing, Loaclizations, WebSettings, SiteWebhooks, and ClientSidePages properties.
| [GetHashCode()](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.1c6872bd.md) | Gets the hash code
| [ToXML(ITemplateFormatter)](OfficeDevPnP.Core.Framework.Provisioning.Model.ProvisioningTemplate.f3da680e.md) | Serializes a template to XML
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
