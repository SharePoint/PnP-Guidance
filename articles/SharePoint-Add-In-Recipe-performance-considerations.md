SharePoint Add-in Recipe - Performance Considerations
=====================================================

Summary
-------

The approaches you take to ensure optimal performance with SharePoint is different in the new SharePoint Add-in model than it was with Full Trust Code.  In a typical Full Trust Code (FTC) / Farm Solution scenario most code operations took place in the SharePoint Server Side Object Model code.

In an SharePoint Add-in model scenario, the SharePoint Client Side Object Model (CSOM) and/or the SharePoint REST API are used to execute code.

The major difference between the two models is server side code versus client side code.  In the SharePoint Add-in model, because code is executed via clients there is additional network traffic which occurs.  Minimizing the API call round trips to the SharePoint server will increase the performance of your SharePoint Add-ins, prevent API throttle limits from being hit, and reduce the amount of resources consumed by your SharePoint site.  

High Level Guidelines
---------------------

As a rule of a thumb, we would like to provide the following high level guidelines to ensure optimal performance with SharePoint in the new SharePoint Add-in model.

- Minimize client side API calls to the SharePoint server.
- Use server side and client side caching techniques to store information.
- It is not recommended to store clientIDs, clientSecrets, Usernames, Passwords, Tokens, or other sensitive security information in caches.

Options to ensure optimal performance with SharePoint
-----------------------------------------------------
You have a couple of options to ensure optimal performance with SharePoint.

- Use client side caching 
- Use server side caching 

Use client side caching 
-----------------------
In this pattern, client side caching techniques such as HTML5 LocalStorage and Cookies are used to cache data.  Information stored in these locations is used to determine if it is necessary to make API calls to a SharePoint server.

- This pattern stores data returned from SharePoint API calls in client side caches.
- This pattern uses client side code (JavaScript) to evaluate data stored in client side caches.
- Cookies are limited to storing 4095 bytes of data.
	+ Cookies have a built in data expiration mechanism.
- HTML5 LocalStorage is limited to 5MB of data.
	- HTML5 LocalStorage does not have a built in data expiration mechanism.  However, such an expiration mechanism may be quickly and easily implemented in JavaScript.
	
		See the **setLocalStorageKeyExpiry** and **isLocalStorageExpired** functions in the [App.js JavaScript file](https://github.com/OfficeDev/PnP/blob/master/Samples/Performance.Caching/Performance.LocalStorage/Scripts/App.js) in the [Performance.LocalStorage (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/master/Samples/Performance.Caching/Performance.LocalStorage) for an example.

**When is it a good fit?**

When you need to use the SharePoint ECMA Client Side Object Model API (sp.js) and evaluate client side data to determine if the API calls need to be made.

**Getting Started**

The [Performance.Caching (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/master/Samples/Performance.Caching) demonstrates how to implement both LocalStorage and Cookie based client side caching in the Add-in model and provides links to several samples and articles.

Use server side caching 
-----------------------
In this pattern, server side caching techniques such as session and server side Cookie evaluation are used to access cached data.  Information stored in these locations is used to determine if it is necessary to make API calls to a SharePoint server.

- This pattern stores data returned from SharePoint API calls in server side caches.
- This pattern uses server side code to evaluate data stored in server side locations.
	+ Server side locations may include session based data, server side caches stored in RAM, or other third party server based caching technologies.
- This pattern uses server side code to evaluate data stored in Cookies.
- Cookies are limited to storing 4095 bytes of data.
	+ Cookies have a built in data expiration mechanism.
	
	See the **CookieCheckSkip** method in the [Customizer.aspx.cs Class](https://github.com/OfficeDev/PnP/blob/master/Solutions/OD4B.Configuration.Async/OD4B.Configuration.AsyncWeb/Pages/Customizer.aspx.cs) in the [OD4B.Configuration.Async (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/master/Solutions/OD4B.Configuration.Async) to see how server side code is used to evaluate Cookies.

**When is it a good fit?**

- When you need to use the SharePoint Managed Code Client Side Object Model API (Microsoft.SharePoint.Client.dll) and evaluate server side data or Cookies to determine if the API calls need to be made.
- When you have long running operations, such as an Azure Web Job, that should only be initiated once per given time frame, no matter how many times a user tries to initiate an operation.  
	+ Applying customized OneDrive for Business configurations are a good example of such a scenario.

**Getting Started**

The [Performance.Caching (O365 PnP Sample)](https://github.com/OfficeDev/PnP/tree/master/Samples/Performance.Caching) describes how to implement both LocalStorage and Cookie based client side caching in the Add-in model and provides links to several samples and articles.

Related links
=============
- Guidance articles at [http://aka.ms/OfficeDevPnPGuidance](http://aka.ms/OfficeDevPnPGuidance "Guidance Articles")
- References in MSDN at [http://aka.ms/OfficeDevPnPMSDN](http://aka.ms/OfficeDevPnPMSDN "References in MSDN")
- Videos at [http://aka.ms/OfficeDevPnPVideos](http://aka.ms/OfficeDevPnPVideos "Videos")

Related PnP samples
===================

- Samples and content at [http://aka.ms/OfficeDevPnP](http://aka.ms/OfficeDevPnP)

Applies to
==========
- Office 365 Multi Tenant (MT)
- Office 365 Dedicated (D)
- SharePoint 2013 on-premises

Author
------
Todd Baginski (Canviz LLC) - [@toddbaginski](https://twitter.com/toddbaginski)

Version history
---------------
Version  | Date | Comments | Author
---------| -----| ---------| ------
0.1  | June 22, 2015 | Initial draft | Todd Baginski
 (Canviz LLC)
