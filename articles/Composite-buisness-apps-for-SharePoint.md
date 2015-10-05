
# Composite business apps for SharePoint 2013 and SharePoint Online
Use composite business apps to integrate your SharePoint solutions with your business processes and technologies. Decide whether a SharePoint-hosted or provider-hosted app is the right choice for your solution.

 **Last modified:** March 16, 2015

 _**Applies to:** Office 365 | SharePoint 2013 | SharePoint Online_

 **In this article**

 [SharePoint-hosted vs. provider-hosted apps](#sectionSection0)

 [In this section](#sectionSection1)

 [Additional resources](#bk_addresources)


Composite business apps are apps that are tightly integrated with your business processes and line-of-business (LOB) technologies (like databases and web services). These apps typically include a number of complex interactions with users and with other technologies.
The sample composite business apps described in this section provide building blocks that you can use to integrate your technologies and processes with the SharePoint 2013 app model.

**Note**  You can [view this article](https://msdn.microsoft.com/EN-US/library/dn957894.aspx) in the [Solutions guidance](https://msdn.microsoft.com/en-us/library/dn904529.aspx) node on MSDN.


## SharePoint-hosted vs. provider-hosted apps
<a name="sectionSection0"> </a>

Before you create composite business apps, you first need to decide where the apps will be hosted. SharePoint-hosted apps work best when you can scope your requirements to single-site implementations that you can handle with JavaScript. Provider-hosted apps are better for more complex business requirements.

The following table summarizes the factors to consider when you decide where to host your apps.

|**SharePoint-hosted apps**|**Provider-hosted apps**|
|:-----|:-----|
|You can do everything you need to do with JavaScript.|You need to use languages other than JavaScript.|
|The app does not need to do any work across more than one site; for example, team calendar apps and featured news rotators.|The app needs to access information and do work across more than a single site. For example, site collection provisioning apps.|
|Content is sensitive and needs to stay securely and entirely in SharePoint.|The app needs to integrate with other line-of-business technologies.|
||The app requires elevated permissions that are made possible by the app-only policy.|
||The app requires a highly customized UI.|



## In this section
<a name="sectionSection1"> </a>

|**Article**|**Sample**|**Shows you how to...**|
|:-----|:-----|:-----|
|[Migrate InfoPath forms to SharePoint 2013](https://msdn.microsoft.com/en-us/library/dn957892.aspx) ||Migrate your InfoPath 2013 forms to other supported technologies.|
|[Data storage options in SharePoint Online](https://msdn.microsoft.com/en-us/library/dn957893.aspx) |[Core.DataStorageModels](https://github.com/OfficeDev/PnP/tree/master/Samples/Core.DataStorageModels) |Use different types of storage models to store your SharePoint Online data.|
|[Corporate event app integration with SharePoint](https://msdn.microsoft.com/en-us/library/dn957895.aspx)|[BusinessApps.CorporateEventsApp](https://github.com/OfficeDev/PnP/tree/master/Solutions/BusinessApps.CorporateEventsApp)|Use a provider-hosted app to implement complex business tasks.|
|[Call web services from SharePoint workflows](https://msdn.microsoft.com/en-us/library/dn957896.aspx)|[Workflow.CallCustomService](https://github.com/OfficeDev/PnP/tree/master/Samples/Workflow.CallCustomService)<br />[Workflow.CallServiceUpdateSPViaProxy](https://github.com/OfficeDev/PnP/tree/master/Samples/Workflow.CallServiceUpdateSPViaProxy)<br />[Workflow.AssociateToHostWeb](https://github.com/OfficeDev/PnP/tree/master/Samples/Workflow.AssociateToHostWeb)|Use provider-hosted apps to call remote web services that contain business data.|

## Additional resources
<a name="bk_addresources"> </a>


-  [Office 365 development patterns and practices solution guidance](http://msdn.microsoft.com/library/4bb8d1ad-1cf9-484c-b444-1aa032608bc1.aspx)
    
-  [Office 365 Development Patterns and Practices on GitHub](https://github.com/OfficeDev/PnP)
    
