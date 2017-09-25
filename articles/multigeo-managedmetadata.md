# Managed metadata in a SharePoint Multi-Geo tenant

> **Important:** OneDrive and SharePoint Online Multi-Geo is currently in preview and is subject to change.

Managed metadata in SharePoint is Multi-Geo aware. This article describes how to manage metadata in a SharePoint Multi-Geo tenant.

The managed metadata that you define for the default geo location of a Multi-Geo tenant automatically replicates to the tenant's satellite locations. Managed metadata that you define for a satellite geo location is only available to the sites that are hosted in that geo location.

**The default location of a Multi-Geo tenant has a special meaning when it comes to managed meta data because the managed meta data you define in the default geo location for your tenant will be automatically replicated to your tenant's satellite locations. If you define managed meta data in one of the geo locations then that managed meta data will only be available for the sites hosted in that geo location.**

Looking at sample below you'll notice that the term groups TGMain1 and TGMain2 which were created in the central location are then replicated to all satellite geo locations, making these terms available throughout the Multi-Geo tenant. Term Sets and Terms synchronization is a 1 way mechanism always flowing from the default location to the satellite locations. Term sets created in a satellite location will not be synchronized to the central location or to any other satellite location, for example term sets created in a satellite geo location (e.g. TGEurope1) will only be available for sites hosted in that geo location (e.g. Europe).

![](/media/multigeo/multigeomanagedmetadata_intro.png)

Here's what you need to know as a developer:

- Replication from the default geo location to any satellite geo location is **one way**. Users can't update the replicated term sets, but administrators can update a replicated term set in a satellite geo location. Note that this however is not recommended as this will result in additional termsets and terms being available in that satellite location
- **It's recommended to only create termgroups, termsets and terms in the default geo location as that will ensure a consistent availability of your enterprise managed metadata across all the geo locations in your tenant**
- When termgroups, termsets and terms are replicated they keep the same id which allows you to reference termgroups, termsets and terms based on their ID, regardless of in which geo location you're code is running
- The replication process runs on an hourly basis for the incremental replication. The full replication job runs each 3 days
- There are no specific API changes around managed meta date: when you programmatically create an termset in the default geo location then that termset will be automatically replicated
- There might be some cases, where you want for a termgroup, termset, or terms to be only available in a satellite location, for example a term relating to a confidential project taking place in that geo location, in these cases, you may choose to create the relevant terms in the applicable geo location. 
- If you want the termgroup to only be available in the default location then you'll need explicitly specify which termgroups from the default location are replicated using the `Set-SPOTenantTaxonomyReplicationParameters` PowerShell cmdlet. This cmdlet is part of the [SharePoint Online Management Shell](https://www.microsoft.com/en-us/download/confirmation.aspx?id=35588).


## Resources
Below list of resources are useful when you're learning more:
- [Information about hybrid managed meta data, but applies as well to a Multi-Geo tenant](https://support.office.com/en-us/article/Plan-hybrid-SharePoint-taxonomy-and-hybrid-content-types-71ae4d00-da98-407b-bee2-8d9972e1875c?ui=en-US&rs=en-US&ad=US)
