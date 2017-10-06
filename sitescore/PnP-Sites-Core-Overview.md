# PnP Sites Core API reference

## Summary
Office 365 Developer PnP Core Component is extension component which encapsulates commonly used remote CSOM/REST operations as reusable [extension methods](http://msdn.microsoft.com/en-us/library/bb383977.aspx) towards out of the box CSOM objects. It's targeted to be used with provider hosted apps or background programs and will help developers to be more efficient and productive by providing single line extension methods for commonly used operations from content type creation to uploading page layouts to publishing sites.

You can learn more about the PnP Core Component from the project [readme file](https://github.com/SharePoint/PnP-Sites-Core/blob/master/Core/README.md). 

## Applies to
-  Office 365 Multi Tenant (MT)
-  Office 365 Dedicated (D)
-  SharePoint 2016 on-premises
-  SharePoint 2013 on-premises


## Namespaces used in the PnP Sites Core library
### OfficeDevPnP.Core namespaces
|**Namespace**|
|:-----|
|[OfficeDevPnP.Core](OfficeDevPnP.Core.md)|
|[OfficeDevPnP.Core.AppModelExtensions](OfficeDevPnP.Core.AppModelExtensions.md)|
|[OfficeDevPnP.Core.Diagnostics](OfficeDevPnP.Core.Diagnostics.md)|
|[OfficeDevPnP.Core.Diagnostics.Tree](OfficeDevPnP.Core.Diagnostics.Tree.md)|
|[OfficeDevPnP.Core.Entities](OfficeDevPnP.Core.Entities.md)|
|[OfficeDevPnP.Core.Enums](OfficeDevPnP.Core.Enums.md)|
|[OfficeDevPnP.Core.Extensions](OfficeDevPnP.Core.Extensions.md)|
|[OfficeDevPnP.Core.Framework.Graph](OfficeDevPnP.Core.Framework.Graph.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.Connectors](OfficeDevPnP.Core.Framework.Provisioning.Connectors.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXML](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXML.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXML.Model](OfficeDevPnP.Core.Framework.Provisioning.Connectors.OpenXML.Model.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.Extensibility](OfficeDevPnP.Core.Framework.Provisioning.Extensibility.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.TokenDefinitions](OfficeDevPnP.Core.Framework.Provisioning.ObjectHandlers.TokenDefinitions.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.Providers.Json](OfficeDevPnP.Core.Framework.Provisioning.Providers.Json.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml](OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.Resolvers](OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.Resolvers.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.V201503](OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.V201503.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.V201505](OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.V201505.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.V201508](OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.V201508.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.V201512](OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.V201512.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.V201605](OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.V201605.md)|
|[OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.V201705](OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.V201705.md)|
|[OfficeDevPnP.Core.Framework.TimerJobs](OfficeDevPnP.Core.Framework.TimerJobs.md)|
|[OfficeDevPnP.Core.Framework.TimerJobs.Enums](OfficeDevPnP.Core.Framework.TimerJobs.Enums.md)|
|[OfficeDevPnP.Core.IdentityModel.TokenProviders.ADFS](OfficeDevPnP.Core.IdentityModel.TokenProviders.ADFS.md)|
|[OfficeDevPnP.Core.IdentityModel.WSTrustBindings](OfficeDevPnP.Core.IdentityModel.WSTrustBindings.md)|
|[OfficeDevPnP.Core.Pages](OfficeDevPnP.Core.Pages.md)|
|[OfficeDevPnP.Core.Sites](OfficeDevPnP.Core.Sites.md)|
|[OfficeDevPnP.Core.UPAWebService](OfficeDevPnP.Core.UPAWebService.md)|
|[OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)|
|[OfficeDevPnP.Core.Utilities.CanvasControl](OfficeDevPnP.Core.Utilities.CanvasControl.md)|
|[OfficeDevPnP.Core.Utilities.CanvasControl.Processors](OfficeDevPnP.Core.Utilities.CanvasControl.Processors.md)|
|[OfficeDevPnP.Core.Utilities.WebParts](OfficeDevPnP.Core.Utilities.WebParts.md)|
|[OfficeDevPnP.Core.Utilities.WebParts.Processors](OfficeDevPnP.Core.Utilities.WebParts.Processors.md)|
|[OfficeDevPnP.Core.Utilities.WebParts.Schema](OfficeDevPnP.Core.Utilities.WebParts.Schema.md)|
|[OfficeDevPnP.Core.WebAPI](OfficeDevPnP.Core.WebAPI.md)|
### Microsoft.SharePoint.Client namespaces
|**Namespace**|
|:-----|
|[Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)|
### System namespaces
|**Namespace**|
|:-----|
|[System](System.md)|



![SharePoint Patterns and Practices](https://devofficecdn.azureedge.net/media/Default/PnP/sppnp.png)

Please use [http://aka.ms/sppnp](http://aka.ms/sppnp) for getting latest information around the whole *Office 365 Developer Patterns and Practices program*.

*"Sharing is Caring"*

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.