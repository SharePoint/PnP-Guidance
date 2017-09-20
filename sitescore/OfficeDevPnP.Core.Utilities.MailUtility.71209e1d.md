# MailUtility.SendEmail Method  
 Sends an email using the SharePoint SendEmail method   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SendEmail(ClientContext context, IEnumerable<String> to, IEnumerable<String> cc, String subject, String body)
```
### Parameters
#### context  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.ClientContext  
&emsp;&emsp;Context for SharePoint objects and operations  

  

#### to  
&emsp;&emsp;Type: System.Collections.Generic.IEnumerable&lt;System.String&gt;  
&emsp;&emsp;List of TO addresses.  

  

#### cc  
&emsp;&emsp;Type: System.Collections.Generic.IEnumerable&lt;System.String&gt;  
&emsp;&emsp;List of CC addresses.  

  

#### subject  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Subject of the mail.  

  

#### body  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;HTML body of the mail.  

  

### Return Value
Type: void  

## See also
- [MailUtility](OfficeDevPnP.Core.Utilities.MailUtility.md) 
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md) 
