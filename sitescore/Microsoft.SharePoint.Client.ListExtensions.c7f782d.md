# ListExtensions.UpdateWebhookSubscription Method  
 Updates a Webhook subscription from the list Note: If the access token is not specified, it will cost a dummy request to retrieve it   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static bool UpdateWebhookSubscription(this List list, Guid subscriptionId, String webHookEndPoint, DateTime expirationDateTime, String accessToken)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;The list to remove the Webhook subscription from  

  

#### subscriptionId  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;The id of the subscription to remove  

  

#### webHookEndPoint  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Url of the web hook service endpoint (the one that will be called during an event)  

  

#### expirationDateTime  
&emsp;&emsp;Type: System.DateTime  
&emsp;&emsp;New web hook expiration date  

  

#### (optional) accessToken  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;(optional) The access token to SharePoint  

  

### Return Value
Type: bool  
 <c>true</c> if the removal succeeded, <c>false</c> otherwise  


## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
