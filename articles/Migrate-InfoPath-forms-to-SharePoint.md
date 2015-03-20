
# Migrate InfoPath forms to SharePoint 2013
Migrate InfoPath forms in your SharePoint apps to other supported solutions, such as Access applications, sandbox solutions, or the app model.

 **Last modified:** March 16, 2015

 _**Applies to:** Office 365 | SharePoint 2013 | SharePoint Online_

If you're using InfoPath as the basis for creating forms in your apps, now is the time to start thinking about migrating your forms to other solutions. Although InfoPath is currently supported, InfoPath 2013 is the last release of the desktop InfoPath client, and InfoPath Forms Services in SharePoint 2013 is the last release of InfoPath Forms Services. The client and the on-premises version of InfoPath Forms Services in SharePoint 2013 will be fully supported until 2023. The forms service will be supported in Office 365 until at least the next major release of Office.

To replace your InfoPath forms, you can choose one of the following alternatives:

- Use Access applications.
    
- Convert InfoPath forms to sandbox solutions.
    
- Move complex behaviors to the app model.
    
We recommend the first two solutions, because information workers who don't know how to write and deploy code-based alternatives can implement them. The following table describes the scenarios for which each alternative is best suited.

 **Alternatives to InfoPath in SharePoint 2013**

|**Alternative**|**Scenario**|
|:-----|:-----|
|Access applications|This option supports multiple forms that handle relational data contained in multiple Access tables, Excel tables, and/or SharePoint lists.|
|Convert InfoPath to Sandbox solutions|This is a viable option if your forms are simple, don’t require any server components, and don’t make any calls to external web services.|
|Convert to the app model|You can convert complex forms driven by extensive code into provider-hosted apps. This option requires developer resources.|

**Note**  You can [view this article](https://msdn.microsoft.com/EN-US/library/dn957892.aspx) in the [Solutions guidance](https://msdn.microsoft.com/en-us/library/dn904529.aspx) node on MSDN.

## Additional resources
<a name="bk_addresources"> </a>


-  [Office 365 development patterns and practices solution guidance](http://msdn.microsoft.com/library/4bb8d1ad-1cf9-484c-b444-1aa032608bc1.aspx)
    
-  [Office 365 Development Patterns and Practices on GitHub](https://github.com/OfficeDev/PnP)
    
