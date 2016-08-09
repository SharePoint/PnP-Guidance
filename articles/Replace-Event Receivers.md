# Replace SharePoint event receivers 
Transform or convert your code-based sandbox solutions to the SharePoint add-in model. Learn about the options and strategies of converting existing functionality to SharePoint add-in model or alternative solutions.

_**Applies to:** Add-ins for SharePoint | SharePoint 2013 | SharePoint 2016 | SharePoint Online_


## Summary

The approach you take to handle events in SharePoint is slightly different in the SharePoint add-in model than it was with Full Trust Code or in coded-sandbox solutions. In typical previous solutions, event receivers were created using the SharePoint Server Side Object Model and deployed via solutions packages, which executes the code on the SharePoint servers. In the SharePoint add-in model; however, the event receiver implementation executes on the web server that is hosting the event receiver and these are called Remote Event Receivers (RER). Event receivers can in many cases be replaced with a remote event receiver implementation. This article describes various options and design considerations.


## Options for replacing Event Receivers
<a name="sectionSection2"> </a>

|**Approach**|**Additional Information**|
|:-----|:-----|
|Remote Event Receiver|</p><lu><li>[Use remote event receivers in SharePoint](https://msdn.microsoft.com/en-us/pnp_articles/use-remote-event-receivers-in-sharepoint)</li><li>[How to use remote event receivers for your SharePoint add-ins](https://channel9.msdn.com/blogs/OfficeDevPnP/How-to-use-remote-event-receivers-for-your-SharePoint-add-ins)</li><li>[Event receivers and list event receivers in the SharePoint add-in model](https://msdn.microsoft.com/en-us/pnp_articles/event-receiver-and-list-event-receiver-sharepoint-add-in)</li></lu><li>[Auto tagging sample add-in for SharePoint](https://msdn.microsoft.com/en-us/pnp_articles/autotagging-sample-app-for-sharepoint)</li><li>[Handle events in SharePoint Add-ins](https://msdn.microsoft.com/en-us/library/office/jj220048.aspx)</li></lu></p>|
|WebHooks|<p>WebHooks  for SharePoint are still under development.<lu><li>[Introducing SharePoint WebHooks](http://dev.office.com/blogs/introducing-sharepoint-webhooks)</li></p>
|Remote Timer Job to monitor changes|<p>Use the **ChangeQuery** object to monitor a site or list for modifications. This pattern is an alternative to Remote Event Receivers<lu><li>[SharePoint List Item Change Monitor](https://github.com/OfficeDev/PnP/tree/master/Samples/Core.ListItemChangeMonitor)</li><li>[Remote Timer Job Pattern](https://github.com/OfficeDev/PnP/tree/master/Samples/Core.SimpleTimerJob)</p>|

## Design Considerations
### Remove Event Receivers
- Requires hosting infrastructure
- Hosting infrastructure must be highly available
- The service endpoint that hosts the remote event receiver must be configured for anonymous authentication
- Requires a trusted 3rd Party certificate if you are using SharePoint Online
- Not intended for long running operations 
- Remote Event Receivers that are attached out-side the context of add-in, attached using a console application or PowerShell; will not receive a SharePoint context token when invoked and you must differ to app-only permissions or use the SharePointOnlineCredentials class
- There is no retry mechanism 


### WebHooks
- Requires hosting infrastructure
- Hosting infrastructure must be highly available
- Does not support synchronous events
- Process changes after the event has occurred
- Public preview available in late 2016


### Remote Timer Job
- Requires hosting infrastructure
- Process changes after the event has occurred
- Uses a polling mechanism to process changes

## Removing your sandbox code from your site
<a name="sectionSection3"> </a>
When you deactivate your existing sandbox solution from sites, any assets or files deployed using declarative options will not be removed. If you have used sandbox solutions to introduce event receivers, upon deactivation of the sandbox solution, the features will automatically be deactivated and the event receiver will be removed from the object.

## Additional Resources
<a name="bk_addresources"> </a>
-  [Removing Code-Based Sandbox Solutions in SharePoint Online](http://dev.office.com/blogs/removing-code-based-sandbox-solutions-in-sharepoint-online)
-  [Sandbox solution transformation guidance](https://msdn.microsoft.com/en-us/pnp_articles/sandbox-solution-transformation-guidance)
-  [Remove assembly reference from your Sandbox solution created in Visual Studio](https://support.microsoft.com/en-us/kb/3183084)
-  [Build add-ins for SharePoint](https://msdn.microsoft.com/library/office/fp179930.aspx)
-  [Office 365 development and SharePoint patterns and practices solution guidance](https://msdn.microsoft.com/en-us/pnp_articles/office-365-development-patterns-and-practices-solution-guidance)
