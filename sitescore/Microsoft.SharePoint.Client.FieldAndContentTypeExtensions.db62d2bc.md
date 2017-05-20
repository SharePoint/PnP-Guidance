# FieldAndContentTypeExtensions.GetFieldByName Method  
  

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  

>**This method is obsolete**
>:Use GetFieldByInternalName instead. This method returns field based on StaticName. This could lead to unexpected results due to StaticName property not necessarily being unique within a field collection. (https://msdn.microsoft.com/en-us/library/microsoft.sharepoint.spfield.staticname.aspx)

## Syntax
```C#
public static Field GetFieldByName(this FieldCollection fields, String internalName)
```
### Parameters
#### fields  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.FieldCollection  
&emsp;&emsp;  

  

#### internalName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;  

  

### Return Value
Type: Field  

## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
