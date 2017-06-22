# XMLSerializer.SerializeToStream Method  
 Serializes an object instance to a stream, providing custom namespace prefixes.   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static Stream SerializeToStream<T>(T objectToSerialize, XmlSerializerNamespaces ns)
```
### Parameters
#### objectToSerialize  
&emsp;&emsp;Type: T  
&emsp;&emsp; Serializes an object instance to a stream, providing custom namespace prefixes.   

  

#### ns  
&emsp;&emsp;Type: System.Xml.Serialization.XmlSerializerNamespaces  
&emsp;&emsp;Xml serializer namespace  

  

### Return Value
Type: Stream  
An string that represents the serialized object.  


## See also
- [XMLSerializer](OfficeDevPnP.Core.Utilities.XMLSerializer.md) 
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md) 
