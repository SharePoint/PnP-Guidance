# TaxonomyExtensions.WireUpTaxonomyField Method  
 Wires up MMS field to the specified term set.   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void WireUpTaxonomyField(this List list, Guid id, String mmsGroupName, String mmsTermSetName, Boolean multiValue = False)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;List to be processed  

  

#### id  
&emsp;&emsp;Type: System.Guid  
&emsp;&emsp;Field ID to be wired up  

  

#### mmsGroupName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Taxonomy group  

  

#### mmsTermSetName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Term set name  

  

#### (optional) multiValue  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Allow multiple selection  

  

### Return Value
Type: void  

## See also
- [TaxonomyExtensions](Microsoft.SharePoint.Client.TaxonomyExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
