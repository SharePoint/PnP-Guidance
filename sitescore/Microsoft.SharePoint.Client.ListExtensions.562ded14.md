# ListExtensions.AddWebhookSubscription Method  
 Add the a Webhook subscription to a list Note: If the access token is not specified, it will cost a dummy request to retrieve it   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static WebhookSubscription AddWebhookSubscription(this List list, String notificationUrl, DateTime expirationDate, String clientState, String accessToken)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;The list to add a Webhook subscription to  

  

#### notificationUrl  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The Webhook endpoint URL  

  

#### expirationDate  
&emsp;&emsp;Type: System.DateTime  
&emsp;&emsp;The expiration date of the subscription  

  

#### (optional) clientState  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The client state to use in the Webhook subscription  

  

#### (optional) accessToken  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;(optional) The access token to SharePoint  

  

### Return Value
Type: [WebhookSubscription](OfficeDevPnP.Core.Entities.WebhookSubscription.md)  
The added subscription object  


## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
