# TreeNodeList&lt;T&gt; Class
 Holds methods for Tree node   

**Namespace:** [OfficeDevPnP.Core.Diagnostics.Tree](OfficeDevPnP.Core.Diagnostics.Tree.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Inheritance Hierarchy
System.Object  
&ensp;OfficeDevPnP.Core.Diagnostics.Tree.ITreeNode  
## Syntax
```C#
public class TreeNodeList<T>: List<ITreeNode<T>>, ITreeNodeList<T>, IList<ITreeNode<T>>, ICollection<ITreeNode<T>>, IEnumerable<ITreeNode<T>>, IEnumerable, INotifyPropertyChanged
```
## Constructors
|**Name**|**Description**|
|:-----|:-----|
| [TreeNodeList(ITreeNode<T>)](OfficeDevPnP.Core.Diagnostics.Tree.TreeNodeList_cdcab78f.ctor1.md) | Constructor 
## Properties
|**Name**|**Description**|
|:-----|:-----|
| [Parent](OfficeDevPnP.Core.Diagnostics.Tree.TreeNodeList_cdcab78f.Parent.md) | Gets or sets Parent node
## Methods
|**Name**|**Description**|
|:-----|:-----|
| [Add(ITreeNode&lt;T&gt;)](OfficeDevPnP.Core.Diagnostics.Tree.TreeNodeList_cdcab78f.19b9df21.md) | Adds node to a tree
| [add_PropertyChanged(PropertyChangedEventHandler)](OfficeDevPnP.Core.Diagnostics.Tree.TreeNodeList_cdcab78f.9af7a0ae.md) | 
| [Remove(ITreeNode&lt;T&gt;)](OfficeDevPnP.Core.Diagnostics.Tree.TreeNodeList_cdcab78f.5be50920.md) | Removes node from a tree
| [remove_PropertyChanged(PropertyChangedEventHandler)](OfficeDevPnP.Core.Diagnostics.Tree.TreeNodeList_cdcab78f.d9af74e7.md) | 
| [ToString()](OfficeDevPnP.Core.Diagnostics.Tree.TreeNodeList_cdcab78f.b40365cf.md) | Retuns count of child nodes as a string
## See also
- [OfficeDevPnP.Core.Diagnostics.Tree](OfficeDevPnP.Core.Diagnostics.Tree.md)
