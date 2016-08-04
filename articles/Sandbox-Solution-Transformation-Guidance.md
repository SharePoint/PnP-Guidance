# Sandbox Solution transformation guidance 
Transform or convert your code-based sandbox solutions to the SharePoint add-in model. Learn about the options and strategies on converting existing code-based functionalities to SharePoint add-in model or alternative solutions.

_**Applies to:** add-ins for SharePoint | SharePoint 2013 | SharePoint Online_

Code-based sandbox solutions [were deprecated](https://blogs.msdn.microsoft.com/sharepointdev/2014/01/14/deprecation-of-custom-code-in-sandboxed-solutions/) back in 2014 and SharePoint online has started the process to completely remove this capability. 

If you have extended your SharePoint Online environment by using code-based sandbox solutions, you'll need to transform away from code-based sandbox solutions, due the deprecation of. Transforming your sandbox solutions to the SharePoint add-in model involves analyzing your existing extensions, designing and developing your new add-in for SharePoint, and then testing and deploying your add-in in your production environment. 

## Steps to perform transformation
<a name="sectionSection0"> </a>

When you transform your sandbox solutions to the SharePoint add-in model, you want to ensure that the impact on your users is minimal. Carefully analyze your current farm solutions, and then design your new add-in for SharePoint to meet the needs of your organization. We recommend the following process to ensure a successful transformation.


1. Readiness. Learn about:
    
	- The SharePoint add-in model, different kinds of add-ins, and hosting options. For more information, see  [Overview of add-ins for SharePoint](https://msdn.microsoft.com/library/office/fp179930.aspx).
    
	- Remote access technologies for accessing your on-premises data.
    
2. Solution assessment. Analyze the functional and business requirements by: 
    
	- Identifying deployed sandbox solutions in your current environment. 
	
	- You can use [specific sandbox solution inventory script](https://github.com/OfficeDev/PnP-Tools/tree/master/Scripts/SharePoint.Sandbox.ListSolutionsFromTenant) provided by the PnP initiative for getting list of installed sandbox solutions in your tenant
    
	- Reviewing requirements with your users. Consider asking your users to demonstrate how they use the existing sandbox solutions to perform their daily work.
    
	- Identifying, documenting, and designing new functionality to include in the new add-in for SharePoint. Consider reviewing your list of new feature requests from your users for additional ideas.
    
	- Identifying unused features, and agreeing with your users to omit this functionality from the new add-in for SharePoint. 
    
	- For each farm solution, determining whether to replace it with an add-in for SharePoint or implement that either using with some out of the box capabilities or other alternative solution.
    
3.  Solution planning. Design the new application using the SharePoint add-in model based on:
    
	- The requirements gathered in step 2.
    
	- Your analysis of the existing code. During your code analysis, consider identifying portions of the code that can be dropped (for example, the code is no longer being used, or the requirements have changed).
    
4. Develop and test the SharePoint add-in model version of your application. 
    
5. Deploy your new add-in. 

## Replacing sandbox solution customizations
<a name="sectionSection1"> </a>

Intro

|**Customization**|**Transformation options**|
|:-----|:-----|
|InfoPath form with code|Deploy your new add-in for SharePoint into your existing SharePoint environment. You need to ensure your site is using the new add-in for SharePoint before retracting the farm solution.|
|Web Part|Web parts are typically converted either to add-in parts or they are implemented with fully client side technologies by using so called JavaScript embed pattern.|
|Event Receiver|Event receivers can in many cases be replaced with the remote event receiver implementation. Remote event receivers do however need to hosted in some platform, typically on specific provider hosted add-in.|
|Feature Receiver|Are typically replaced with a remote API based operation, like using CSOM or REST for applying the needed customization|
|Custom workflow action|Typical code migration path for these kind of customizations is to start using either SharePoint 2013 workflows or to move using alternative solutions, like Microsoft Flow.|

We are looking for adding specific articles on the transformation techniques for specific topics. 

## Removing your sandbox code
<a name="sectionSection1"> </a>
Intro

## Additional resources
<a name="bk_addresources"> </a>

-  [Removing Code-Based Sandbox Solutions in SharePoint Online](http://dev.office.com/blogs/removing-code-based-sandbox-solutions-in-sharepoint-online)

-  [Remove assembly reference from your Sandbox solution created in Visual Studio](https://support.microsoft.com/en-us/kb/3183084)

-  [Office 365 development patterns and practices solution guidance](Office-365-development-patterns-and-practices-solution-guidance.md)
    
-  [Build add-ins for SharePoint](https://msdn.microsoft.com/library/jj163230.aspx)
