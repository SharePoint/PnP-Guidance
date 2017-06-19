# ListExtensions.SetDefaultColumnValues Method  


Sets default values for column values.

In order to for instance set the default Enterprise Metadata keyword field to a term, add the enterprise metadata keyword to a library (internal name "TaxKeyword")



Column values are defined by the DefaultColumnValue class that has 3 properties:

RelativeFolderPath : / to set a default value for the root of the document library, or /foldername to specify a subfolder

FieldInternalName : The name of the field to set. For instance "TaxKeyword" to set the Enterprise Metadata field

Terms : A collection of Taxonomy terms to set



Supported column types: Metadata, Text, Choice, MultiChoice, People, Boolean, DateTime, Number, Currency  

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetDefaultColumnValues(this List list, IEnumerable<IDefaultColumnValue> columnValues)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;List to process  

  

#### columnValues  
&emsp;&emsp;Type: System.Collections.Generic.IEnumerable&lt;OfficeDevPnP.Core.Entities.IDefaultColumnValue&gt;  
&emsp;&emsp;Column Values  

  

### Return Value
Type: void  

## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
