# WebExtensions.CreateWeb Method  
 Adds a new child Web (site) to a parent Web.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Web CreateWeb(this Web parentWeb, String title, String leafUrl, String description, String template, Int32 language, Boolean inheritPermissions = True, Boolean inheritNavigation = True)
```
### Parameters
#### parentWeb  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The parent Web (site) to create under  

  

#### title  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The title of the new site.   

  

#### leafUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;A string that represents the URL leaf name.  

  

#### description  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The description of the new site.   

  

#### template  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The name of the site template to be used for creating the new site.   

  

#### language  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;The locale ID that specifies the language of the new site.   

  

#### (optional) inheritPermissions  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Specifies whether the new site will inherit permissions from its parent site.  

  

#### (optional) inheritNavigation  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Specifies whether the site inherits navigation.  

  

### Return Value
Type: Web  

## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
