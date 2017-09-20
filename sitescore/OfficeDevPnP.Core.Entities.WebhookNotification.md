# WebhookNotification Class
 Web hook notification model: this message is received when SharePoint "fires" a web hook   

**Namespace:** [OfficeDevPnP.Core.Entities](OfficeDevPnP.Core.Entities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public class WebhookNotification
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [WebhookNotification()](OfficeDevPnP.Core.Entities.WebhookNotification.ctor1.md) |  Web hook notification model: this message is received when SharePoint "fires" a web hook 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [ClientState](OfficeDevPnP.Core.Entities.WebhookNotification.ClientState.md) | An opaque string passed back to the client on all notifications. You can use this for validating notifications, tagging different subscriptions, or other reasons.
| [ExpirationDateTime](OfficeDevPnP.Core.Entities.WebhookNotification.ExpirationDateTime.md) | The expiration date for subscription. The expiration date should not be more than 6 months. By default, subscriptions are set to expire 6 months from when they are created.
| [Resource](OfficeDevPnP.Core.Entities.WebhookNotification.Resource.md) | The resource endpoint URL you are creating the subscription for. For example a SharePoint List API URL
| [SiteUrl](OfficeDevPnP.Core.Entities.WebhookNotification.SiteUrl.md) | SharePoint site url
| [SubscriptionId](OfficeDevPnP.Core.Entities.WebhookNotification.SubscriptionId.md) | Webhook subscription id
| [TenantId](OfficeDevPnP.Core.Entities.WebhookNotification.TenantId.md) | SharePoint tenant id
| [WebId](OfficeDevPnP.Core.Entities.WebhookNotification.WebId.md) | SharePoint web id
## See also
- [OfficeDevPnP.Core.Entities](OfficeDevPnP.Core.Entities.md)
