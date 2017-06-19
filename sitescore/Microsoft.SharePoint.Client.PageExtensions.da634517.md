# PageExtensions.SetWebPartProperty Method  
 Sets a web part property   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetWebPartProperty(this Web web, String key, Int32 value, Guid id, String serverRelativePageUrl)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The web to process  

  

#### key  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The key to update  

  

#### value  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;The value to set  

  

#### id  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;The id of the webpart  

  

#### serverRelativePageUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Server relative url of the page to set web part property  

  

### Return Value
Type: void  

## See also
- [PageExtensions](Microsoft.SharePoint.Client.PageExtensions.md) 
- System.ArgumentException
- System.ArgumentNullException
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
