# Webhook Class
 Defines a Webhook   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;[OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel](OfficeDevPnP.Core.Framework.Provisioning.Model.BaseModel.md)  
## Syntax
```C#
public class Webhook: BaseModel, IEquatable<Webhook>
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [Webhook()](OfficeDevPnP.Core.Framework.Provisioning.Model.Webhook.ctor1.md) |  Defines a Webhook 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [ExpiresInDays](OfficeDevPnP.Core.Framework.Provisioning.Model.Webhook.ExpiresInDays.md) | Defines the expire days for the subscription of the Webhook, required attribute.
| [ServerNotificationUrl](OfficeDevPnP.Core.Framework.Provisioning.Model.Webhook.ServerNotificationUrl.md) | Defines the Server Notification URL of the Webhook, required attribute.
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Equals(Object)](OfficeDevPnP.Core.Framework.Provisioning.Model.Webhook.3520ddbb.md) | Compares object with Webhook class
| [Equals(Webhook)](OfficeDevPnP.Core.Framework.Provisioning.Model.Webhook.be69e809.md) | Compares Webhook object based on ServerNotificationUrl and ExpiresInDays
| [GetHashCode()](OfficeDevPnP.Core.Framework.Provisioning.Model.Webhook.1c6872bd.md) | Gets the hash code
## See also
- [OfficeDevPnP.Core.Framework.Provisioning.Model](OfficeDevPnP.Core.Framework.Provisioning.Model.md)
