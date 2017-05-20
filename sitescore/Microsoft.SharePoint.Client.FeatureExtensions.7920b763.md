# FeatureExtensions.DeactivateFeature Method  
 Deactivates a site collection or site scoped feature   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void DeactivateFeature(this Site site, Guid featureID, Int32 pollingIntervalSeconds = 30)
```
### Parameters
#### site  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.Site  
&emsp;&emsp;Site to be processed  

  

#### featureID  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;ID of the feature to deactivate  

  

#### (optional) pollingIntervalSeconds  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;The time in seconds between polls for "IsActive"  

  

### Return Value
Type: void  

## See also
- [FeatureExtensions](Microsoft.SharePoint.Client.FeatureExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
