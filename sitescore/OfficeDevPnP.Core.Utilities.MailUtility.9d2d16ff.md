# MailUtility.SendEmail Method  
 Sends an email via Office 365 SMTP   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SendEmail(String servername, String fromAddress, String fromUserPassword, IEnumerable<String> to, IEnumerable<String> cc, String subject, String body, Boolean sendAsync = False, Object asyncUserToken)
```
### Parameters
#### servername  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Office 365 SMTP address. By default this is smtp.office365.com.  

  

#### fromAddress  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The user setting up the SMTP connection. This user must have an EXO license.  

  

#### fromUserPassword  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;The password of the user.  

  

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

  

#### (optional) sendAsync  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Sends the email asynchronous so as to not block the current thread (default: false).  

  

#### (optional) asyncUserToken  
&emsp;&emsp;Type: System.Object  
&emsp;&emsp;The user token that is used to correlate the asynchronous email message.  

  

### Return Value
Type: void  

## See also
- [MailUtility](OfficeDevPnP.Core.Utilities.MailUtility.md) 
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md) 
