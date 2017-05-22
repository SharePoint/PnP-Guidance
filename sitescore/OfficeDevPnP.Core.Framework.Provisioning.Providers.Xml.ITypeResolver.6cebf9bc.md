# ITypeResolver.Resolve Method  
 Resolves a source type into a result   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml](OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public abstract object Resolve(Object source, Dictionary<String, IResolver> resolvers, Boolean recursive = False)
```
### Parameters
#### source  
&emsp;&emsp;Type: System.Object  
&emsp;&emsp;The full source object to resolve  

  

#### (optional) resolvers  
&emsp;&emsp;Type: System.Collections.Generic.Dictionary&lt;System.String, OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.IResolver&gt;  
&emsp;&emsp; Resolves a source type into a result   

  

#### (optional) recursive  
&emsp;&emsp;Type: System.Boolean  
&emsp;&emsp;Defines whether to apply the mapping recursively, optional and by default false  

  

### Return Value
Type: object  

## See also
- [ITypeResolver](OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.ITypeResolver.md) 
- [OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml](OfficeDevPnP.Core.Framework.Provisioning.Providers.Xml.md) 
