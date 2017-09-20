# TenantExtensions.CreateSiteCollection Method  
 Launches a site collection creation and waits for the creation to finish   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Guid CreateSiteCollection(this Tenant tenant, String siteFullUrl, String title, String siteOwnerLogin, String template, Int32 storageMaximumLevel, Int32 storageWarningLevel, Int32 timeZoneId, Int32 userCodeMaximumLevel, Int32 userCodeWarningLevel, UInt32 lcid, Boolean removeFromRecycleBin = False, Boolean wait = True, Func<TenantOperationMessage, Boolean> timeoutFunction)
```
### Parameters
#### tenant  
&emsp;&emsp;Type: Microsoft.Online.SharePoint.TenantAdministration.Tenant  
&emsp;&emsp;A tenant object pointing to the context of a Tenant Administration site  

  

#### siteFullUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The SPO url  

  

#### title  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The site title  

  

#### siteOwnerLogin  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Owner account  

  

#### template  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Site template being used  

  

#### storageMaximumLevel  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Site quota in MB  

  

#### storageWarningLevel  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;Site quota warning level in MB  

  

#### timeZoneId  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;TimeZoneID for the site. "(UTC+01:00) Brussels, Copenhagen, Madrid, Paris" = 3   

  

#### userCodeMaximumLevel  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;The user code quota in points  

  

#### userCodeWarningLevel  
&emsp;&emsp;Type: System.Int32  
&emsp;&emsp;The user code quota warning level in points  

  

#### lcid  
&emsp;&emsp;Type: System.UInt32  
&emsp;&emsp;The site locale. See http://technet.microsoft.com/en-us/library/ff463597.aspx for a complete list of Lcid's  

  

#### (optional) removeFromRecycleBin  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;If true, any existing site with the same URL will be removed from the recycle bin  

  

#### (optional) wait  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Wait for the site to be created before continuing processing  

  

#### (optional) timeoutFunction  
&emsp;&emsp;Type: System.Func&lt;OfficeDevPnP.Core.TenantOperationMessage, System.Boolean&gt;  
&emsp;&emsp;An optional function that will be called while waiting for the site to be created. If set will override the wait variable. Return true to cancel the wait loop.  

  

### Return Value
Type: Guid  
Guid of the created site collection and Guid.Empty is the wait parameter is specified as false. Returns Guid.Empty if the wait is cancelled.  


## See also
- [TenantExtensions](Microsoft.SharePoint.Client.TenantExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
