# WebAPIHelper.RegisterWebAPIService Method  
 This method needs to be called from a code behind of the SharePoint app startup page (default.aspx). It registers the calling SharePoint app by calling a specific "Register" api in your WebAPI service. Note: Given that method is async you'll need to add the Async="true" page directive to the page that uses this method.   

**Namespace:** [OfficeDevPnP.Core.WebAPI](OfficeDevPnP.Core.WebAPI.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void RegisterWebAPIService(HttpContextBase context, String apiRequest, Uri serviceEndPoint)
```
### Parameters
#### context  
&emsp;&emsp;Type: System.Web.HttpContextBase  
&emsp;&emsp;The HttpContextBase object, needed to insert the services token cookie and read the querystring  

  

#### apiRequest  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Route to the "Register" API  

  

#### (optional) serviceEndPoint  
&emsp;&emsp;Type: System.Uri  
&emsp;&emsp;Optional Uri to the WebAPI service endpoint. If null then the assumption is taken that the WebAPI is hosted together with the page making this call  

  

### Return Value
Type: void  

## See also
- [WebAPIHelper](OfficeDevPnP.Core.WebAPI.WebAPIHelper.md) 
- [OfficeDevPnP.Core.WebAPI](OfficeDevPnP.Core.WebAPI.md) 
