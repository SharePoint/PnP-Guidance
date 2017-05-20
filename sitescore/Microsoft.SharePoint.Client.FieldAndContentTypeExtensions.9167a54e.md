# FieldAndContentTypeExtensions.CreateField Method  
  

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static TField CreateField<TField>(this List list, FieldCreationInformation fieldCreationInformation, Boolean executeQuery = True) where TField : Field
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;  

  

#### fieldCreationInformation  
&emsp;&emsp;Type: [OfficeDevPnP.Core.Entities.FieldCreationInformation](OfficeDevPnP.Core.Entities.FieldCreationInformation.md)  
&emsp;&emsp;  

  

#### (optional) executeQuery  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;  

  

### Return Value
Type: TField  

## See also
- [FieldAndContentTypeExtensions](Microsoft.SharePoint.Client.FieldAndContentTypeExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
