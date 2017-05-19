# MailUtility.SendEmailAsync Method  
 Sends an email via Office 365 SMTP as an asynchronous operation   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Task SendEmailAsync(String servername, String fromAddress, String fromUserPassword, IEnumerable<String> to, IEnumerable<String> cc, String subject, String body)
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

  

### Return Value
Type: Task  

## See also
- [MailUtility](OfficeDevPnP.Core.Utilities.MailUtility.md) 
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md) 
