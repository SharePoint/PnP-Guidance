# Replace SharePoint event receivers
Transform or convert your code-based sandbox solutions to the SharePoint add-in model. Learn about the options and strategies of converting existing functionlity to SharePoint add-in model or alternative solutions.

_**Applies to:** Add-ins for SharePoint | SharePoint 2013 | SharePoint 2016 | SharePoint Online_


## Summary

Code-based sandbox solutions [were deprecated](https://blogs.msdn.microsoft.com/sharepointdev/2014/01/14/deprecation-of-custom-code-in-sandboxed-solutions/) back in 2014 and SharePoint online has started the process to completely remove this capability. Code-based sandbox solutions are also deprecated in SharePoint 2013 and SharePoint 2016.

The approach you take to handle events in SharePoint is sightly different in the SharePoint Add-in model than it was with Full Trust Code or in coded-sandbox solutions. In typical sandbox solutions, event receivers were created with the SharePoint Server Side Object Model code and deployed via solutions packages, which executes the code on the SharePoint servers. In the SharePoint add-in model; however, the event receiver implementation executes on the web server that is hosting the event receiver and these are called Remote Event Receivers (RER). Event receivers can in many cases be replaced with an remote event receiver implementation.


## Replacing event receivers options
<a name="sectionSection2"> </a>

|**Option**|**Transformation options**|
|:-----|:-----|
|Event Receiver|<p>Event receivers can in many cases be replaced with the remote event receiver implementation. Remote event receivers do however need to hosted in some platform, typically on specific provider hosted add-in.</p><p>See following resources for additional information <lu><li>[Use remote event receivers in SharePoint](https://msdn.microsoft.com/en-us/pnp_articles/use-remote-event-receivers-in-sharepoint)</li><li>[How to use remote event receivers for your SharePoint add-ins](https://channel9.msdn.com/blogs/OfficeDevPnP/How-to-use-remote-event-receivers-for-your-SharePoint-add-ins)</li></lu></p>|

## Removing your sandbox code  from your site
<a name="sectionSection3"> </a>
When you deactivate your existing sandbox solution from sites, any assets or files deployed using declarative options will not be removed. If you have used sandbox solutions to introduce new code-based web parts, those functionalities will be disabled from the sites. This means that the pages are still rendering normally, so there's no direct end user impact when solution is deactivated, except removal of the code-based functionalities, like web parts.

## Additional resources
<a name="bk_addresources"> </a>

-  [Removing Code-Based Sandbox Solutions in SharePoint Online](http://dev.office.com/blogs/removing-code-based-sandbox-solutions-in-sharepoint-online)
-  [Remove assembly reference from your Sandbox solution created in Visual Studio](https://support.microsoft.com/en-us/kb/3183084)
-  [Event receivers and list event receivers in the SharePoint add-in model](https://msdn.microsoft.com/en-us/pnp_articles/event-receiver-and-list-event-receiver-sharepoint-add-in)


## NOTE    
THIS ARTICLE IS IN PROGRESS 