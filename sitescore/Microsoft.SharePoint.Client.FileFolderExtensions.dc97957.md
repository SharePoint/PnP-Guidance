# FileFolderExtensions.SetFileProperties Method  
 Sets file properties using a dictionary.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetFileProperties(this File file, IDictionary<String, String> properties, Boolean checkoutIfRequired = True)
```
### Parameters
#### file  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.File  
&emsp;&emsp;Target file object.  

  

#### properties  
&emsp;&emsp;Type: System.Collections.Generic.IDictionary&lt;System.String, System.String&gt;  
&emsp;&emsp;Dictionary of properties to set.  

  

#### (optional) checkoutIfRequired  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Check out the file if necessary to set properties.  

  

### Return Value
Type: void  

## See also
- [FileFolderExtensions](Microsoft.SharePoint.Client.FileFolderExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
