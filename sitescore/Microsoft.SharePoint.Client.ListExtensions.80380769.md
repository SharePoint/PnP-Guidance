# ListExtensions.SetLocalizationLabelsForList Method  
 Can be used to set translations for different cultures.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetLocalizationLabelsForList(this Web web, String listTitle, String cultureName, String titleResource, String descriptionResource)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;Site to be processed - can be root web or sub site  

  

#### listTitle  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Title of the list  

  

#### cultureName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Culture name like en-us or fi-fi  

  

#### titleResource  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Localized Title string  

  

#### descriptionResource  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Localized Description string  

  

### Return Value
Type: void  

## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [http://blogs.msdn.com/b/vesku/archive/2014/03/20/office365-multilingual-content-types-site-columns-and-site-other-elements.aspx](http://blogs.msdn.com/b/vesku/archive/2014/03/20/office365-multilingual-content-types-site-columns-and-site-other-elements.aspx)
- System.ArgumentException
- System.ArgumentNullException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
