# ITemplateProviderExtension.PostProcessSaveTemplate Method  
 Method invoked after serializing the template and before it is saved onto the target repository   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public abstract Stream PostProcessSaveTemplate(Stream stream)
```
### Parameters
#### stream  
&emsp;&emsp;Type: System.IO.Stream  
&emsp;&emsp;The source stream  

  

### Return Value
Type: Stream  
The resulting stream, after pre-processing  


## See also
- [ITemplateProviderExtension](OfficeDevPnP.Core.Framework.Provisioning.Providers.ITemplateProviderExtension.md) 
- [OfficeDevPnP.Core.Framework.Provisioning.Providers](OfficeDevPnP.Core.Framework.Provisioning.Providers.md) 
