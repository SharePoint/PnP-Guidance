# ListExtensions.GetWebhookSubscriptions Method  
 Get all the existing Webhooks subscriptions of the list Note: If the access token is not specified, it will cost a dummy request to retrieve it   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static IList<WebhookSubscription> GetWebhookSubscriptions(this List list, String accessToken)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;The list to get the subscriptions of  

  

#### (optional) accessToken  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;(optional) The access token to SharePoint  

  

### Return Value
Type: IList<WebhookSubscription>  
The collection of Webhooks subscriptions of the list  


## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
