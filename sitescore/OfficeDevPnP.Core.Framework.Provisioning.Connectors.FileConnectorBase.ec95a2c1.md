# FileConnectorBase.SaveFileStream Method  
 Saves a stream to the specified container with the given name. If the file exists it will be overwritten   

**Namespace:** [OfficeDevPnP.Core.Framework.Provisioning.Connectors](OfficeDevPnP.Core.Framework.Provisioning.Connectors.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public abstract void SaveFileStream(String fileName, String container, Stream stream)
```
### Parameters
#### fileName  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the file to save  

  

#### container  
&emsp;&emsp;Type: System.String  
&emsp;&emsp;Name of the container to save the file to  

  

#### stream  
&emsp;&emsp;Type: System.IO.Stream  
&emsp;&emsp;Stream containing the file contents  

  

### Return Value
Type: void  

## See also
- [FileConnectorBase](OfficeDevPnP.Core.Framework.Provisioning.Connectors.FileConnectorBase.md) 
- [OfficeDevPnP.Core.Framework.Provisioning.Connectors](OfficeDevPnP.Core.Framework.Provisioning.Connectors.md) 
