# Content type hub in a Multi-Geo tenant

> **Important:** OneDrive and SharePoint Online Multi-Geo is currently in preview and is subject to change.

Customers use the content type hub to have a central place to define content types and then publish these to all sites in the tenant. Below we will cover how content type hubs work in a Multi-Geo tenant.

## Using content type hub in a Multi-Geo tenant
In a Multi-Geo tenant there is a content type hub per geo location, which means you can define content types in each geo region by going to the following site, create the needed content types and publish them.

```
https://<tenant>.sharepoint.com/sites/contenttypehub
```

There's however an important distinction between the content type hub in the default geo location and in the satellite geo location(s): **when you create and publish a content type in the default geo location content type hub then that content type will be available in all sites in your tenant, regardless of which geo location the site is hosted in.** Below picture is showing that content types created in the North America geo location, which is the default locations for this tenant, (so contenttype1 and contenttype2) will be pushed to all sites across the satellite geo locations for the tenant while content types created in the Europe (which is a satellite locations for this tenant) content type hub (contenttype3 and contenttype4) will only be pushed to the sites in the European geo location.

![World map showing content types across geo locations](media/multigeo/multigeocontenttypehub_intro.png)

> **Recommendation**
> - Given enterprises want to have content types being consistent across their tenant it's a best practice to only use the content type hub in the default geo location for creation and publishing of content types. If you do not want all content types of the default location content type hub to be published to all geo locations then you can use the `Set-SPOTenantContentTypeReplicationParameters` PowerShell cmdlet to configure the content types that you do want to publish. This cmdlet is part of the [SharePoint Online Management Shell](https://www.microsoft.com/en-us/download/confirmation.aspx?id=35588).
> - Alternative to using a content type hub enterprises can also integrate the provisioning of content types in their site provisioning solutions: this offers more flexibility and can be realized as fully automated provisioning flow.

## Resources
Use below resources to learn more about content type hub:
- [Content type hub introduction](https://support.office.com/en-US/article/Introduction-to-content-types-and-content-type-publishing-E1277A2E-A1E8-4473-9126-91A0647766E5#__toc256601764)

