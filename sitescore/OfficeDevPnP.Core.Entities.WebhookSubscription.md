# WebhookSubscription Class
 Represents the payload of a Http message   

**Namespace:** [OfficeDevPnP.Core.Entities](OfficeDevPnP.Core.Entities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public class WebhookSubscription
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [WebhookSubscription()](OfficeDevPnP.Core.Entities.WebhookSubscription.ctor1.md) |  Represents the payload of a Http message 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [ClientState](OfficeDevPnP.Core.Entities.WebhookSubscription.ClientState.md) | An opaque string passed back to the client on all notifications. You can use this for validating notifications, tagging different subscriptions, or other reasons.
| [ExpirationDateTime](OfficeDevPnP.Core.Entities.WebhookSubscription.ExpirationDateTime.md) | The expiration date for subscription. The expiration date should not be more than 6 months. By default, subscriptions are set to expire 6 months from when they are created.
| [Id](OfficeDevPnP.Core.Entities.WebhookSubscription.Id.md) | Webhook subscription id
| [NotificationUrl](OfficeDevPnP.Core.Entities.WebhookSubscription.NotificationUrl.md) | Webhook notification url
| [Resource](OfficeDevPnP.Core.Entities.WebhookSubscription.Resource.md) | The resource endpoint URL you are creating the subscription for. For example a SharePoint List API URL
## See also
- [OfficeDevPnP.Core.Entities](OfficeDevPnP.Core.Entities.md)
