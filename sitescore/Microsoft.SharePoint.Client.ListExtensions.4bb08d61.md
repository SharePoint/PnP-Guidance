# ListExtensions.SetDefaultColumnValues Method  
 &lt;para&gt;Sets default values for column values.&lt;/para&gt; &lt;para&gt;In order to for instance set the default Enterprise Metadata keyword field to a term, add the enterprise metadata keyword to a library (internal name "TaxKeyword")&lt;/para&gt; &lt;para&gt;&lt;/para&gt; &lt;para&gt;Column values are defined by the DefaultColumnValue class that has 3 properties:&lt;/para&gt; &lt;para&gt;RelativeFolderPath : / to set a default value for the root of the document library, or /foldername to specify a subfolder&lt;/para&gt; &lt;para&gt;FieldInternalName : The name of the field to set. For instance "TaxKeyword" to set the Enterprise Metadata field&lt;/para&gt; &lt;para&gt;Terms : A collection of Taxonomy terms to set&lt;/para&gt; &lt;para&gt;&lt;/para&gt; &lt;para&gt;Supported column types: Metadata, Text, Choice, MultiChoice, People, Boolean, DateTime, Number, Currency&lt;/para&gt;   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetDefaultColumnValues(List list, IEnumerable<IDefaultColumnValue> columnValues)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp; &lt;para&gt;Sets default values for column values.&lt;/para&gt; &lt;para&gt;In order to for instance set the default Enterprise Metadata keyword field to a term, add the enterprise metadata keyword to a library (internal name "TaxKeyword")&lt;/para&gt; &lt;para&gt;&lt;/para&gt; &lt;para&gt;Column values are defined by the DefaultColumnValue class that has 3 properties:&lt;/para&gt; &lt;para&gt;RelativeFolderPath : / to set a default value for the root of the document library, or /foldername to specify a subfolder&lt;/para&gt; &lt;para&gt;FieldInternalName : The name of the field to set. For instance "TaxKeyword" to set the Enterprise Metadata field&lt;/para&gt; &lt;para&gt;Terms : A collection of Taxonomy terms to set&lt;/para&gt; &lt;para&gt;&lt;/para&gt; &lt;para&gt;Supported column types: Metadata, Text, Choice, MultiChoice, People, Boolean, DateTime, Number, Currency&lt;/para&gt;   

  

#### columnValues  
&emsp;&emsp;Type: System.Collections.Generic.IEnumerable<OfficeDevPnP.Core.Entities.IDefaultColumnValue>  
&emsp;&emsp; &lt;para&gt;Sets default values for column values.&lt;/para&gt; &lt;para&gt;In order to for instance set the default Enterprise Metadata keyword field to a term, add the enterprise metadata keyword to a library (internal name "TaxKeyword")&lt;/para&gt; &lt;para&gt;&lt;/para&gt; &lt;para&gt;Column values are defined by the DefaultColumnValue class that has 3 properties:&lt;/para&gt; &lt;para&gt;RelativeFolderPath : / to set a default value for the root of the document library, or /foldername to specify a subfolder&lt;/para&gt; &lt;para&gt;FieldInternalName : The name of the field to set. For instance "TaxKeyword" to set the Enterprise Metadata field&lt;/para&gt; &lt;para&gt;Terms : A collection of Taxonomy terms to set&lt;/para&gt; &lt;para&gt;&lt;/para&gt; &lt;para&gt;Supported column types: Metadata, Text, Choice, MultiChoice, People, Boolean, DateTime, Number, Currency&lt;/para&gt;   

  

### Return Value
Type: void  

## Remarks
  
## See also
- [ListExtensions](Microsoft.SharePoint.Client.ListExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
