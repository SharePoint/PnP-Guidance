# CAML Class
 Use this class to build your CAML xml and avoid XML issues.   

**Namespace:** [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
## Syntax
```C#
public static class CAML
```
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [And(String, String[])](OfficeDevPnP.Core.Utilities.CAML.2163f362.md) | 
| [BeginsWith(String)](OfficeDevPnP.Core.Utilities.CAML.98c94c83.md) | 
| [Contains(String)](OfficeDevPnP.Core.Utilities.CAML.30c4004e.md) | 
| [DateRangesOverlap(String)](OfficeDevPnP.Core.Utilities.CAML.3b844ec8.md) | 
| [Eq(String)](OfficeDevPnP.Core.Utilities.CAML.b61163fe.md) | 
| [FieldRef(String)](OfficeDevPnP.Core.Utilities.CAML.145eb1c6.md) | Creates a &lt;FieldRef&gt; node for ViewFields clause
| [FieldValue(String, String, String, String)](OfficeDevPnP.Core.Utilities.CAML.d591550d.md) | Creates both a &lt;FieldRef&gt; and &lt;Value&gt; nodes combination for Where clauses.
| [FieldValue(Guid, String, String, String)](OfficeDevPnP.Core.Utilities.CAML.e7e6d57b.md) | Creates both a &lt;FieldRef&gt; and &lt;Value&gt; nodes combination for Where clauses.
| [Geq(String)](OfficeDevPnP.Core.Utilities.CAML.ee6386e1.md) | 
| [Gt(String)](OfficeDevPnP.Core.Utilities.CAML.b5706338.md) | 
| [In(String)](OfficeDevPnP.Core.Utilities.CAML.b4b6656a.md) | 
| [Includes(String)](OfficeDevPnP.Core.Utilities.CAML.675847ac.md) | 
| [IsNotNull(String)](OfficeDevPnP.Core.Utilities.CAML.24458b05.md) | 
| [IsNull(String)](OfficeDevPnP.Core.Utilities.CAML.f92d91c8.md) | 
| [Leq(String)](OfficeDevPnP.Core.Utilities.CAML.ee63bade.md) | 
| [Lt(String)](OfficeDevPnP.Core.Utilities.CAML.b57064c7.md) | 
| [Neq(String)](OfficeDevPnP.Core.Utilities.CAML.ee63a4f8.md) | 
| [NotIncludes(String)](OfficeDevPnP.Core.Utilities.CAML.1518f754.md) | 
| [Or(String, String[])](OfficeDevPnP.Core.Utilities.CAML.d687337d.md) | 
| [OrderBy(OrderByField[])](OfficeDevPnP.Core.Utilities.CAML.e8e4df3.md) | 
| [Today(Nullable&lt;Int32&gt;)](OfficeDevPnP.Core.Utilities.CAML.964aa169.md) | Creates the &lt;Today /&gt; node.
| [ViewFields(String[])](OfficeDevPnP.Core.Utilities.CAML.4f215fe4.md) | 
| [ViewQuery(String, String, Int32)](OfficeDevPnP.Core.Utilities.CAML.ca539507.md) | Root &lt;View&gt; and &lt;Query&gt; nodes.
| [ViewQuery(ViewScope, String, String, String, Int32)](OfficeDevPnP.Core.Utilities.CAML.eb386895.md) | Root &lt;View&gt; and &lt;Query&gt; nodes.
| [Where(String)](OfficeDevPnP.Core.Utilities.CAML.93c72eea.md) | 
## Examples
```C#
CAML.ViewQuery(
    CAML.Where(
        CAML.And(
            CAML.Eq(CAML.FieldValue("Project", "Integer", "{0}")),
            CAML.Geq(CAML.FieldValue("StartDate","DateTime", CAML.Today()))
        )
    ),
    CAML.OrderBy(
        new OrderByField("StartDate", false),
        new OrderByField("Title")
    ),
    rowLimit: 5
);
```

## See also
- [OfficeDevPnP.Core.Utilities](OfficeDevPnP.Core.Utilities.md)
