# WebExtensions.GetAllWebUrls Method  
 Gets the collection of the URLs of all Web sites that are contained within the site collection, including the top-level site and its subsites.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static IEnumerable<String> GetAllWebUrls(this Site site)
```
### Parameters
#### site  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Site  
&emsp;&emsp;Site collection to retrieve the URLs for.  

  

### Return Value
Type: IEnumerable<String>  
An enumeration containing the full URLs as strings.  


## Remarks
 This is analagous to the SPSite.AllWebs property and can be used to get a collection of all web site URLs to loop through, e.g. for branding. 
  
## See also
- [WebExtensions](Microsoft.SharePoint.Client.WebExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
