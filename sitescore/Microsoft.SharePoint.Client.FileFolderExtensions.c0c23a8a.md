# FileFolderExtensions.CheckInFile Method  
 Checks in a file   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void CheckInFile(this Web web, String serverRelativeUrl, CheckinType checkinType, String comment)
```
### Parameters
#### web  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Web  
&emsp;&emsp;The web to process  

  

#### serverRelativeUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The server relative url of the file to checkin  

  

#### checkinType  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.CheckinType  
&emsp;&emsp;The type of the checkin  

  

#### comment  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Message to be recorded with the approval  

  

### Return Value
Type: void  

## See also
- [FileFolderExtensions](Microsoft.SharePoint.Client.FileFolderExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
