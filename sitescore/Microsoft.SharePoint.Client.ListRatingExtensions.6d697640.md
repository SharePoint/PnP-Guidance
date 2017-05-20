# ListRatingExtensions.SetRating Method  
 Enable Social Settings Likes/Ratings on list. Note: 1. Requires Publishing feature enabled on the web. 2. Defaults enable Ratings Experience on the List 3. When experience set to None, fields are not removed from the list since CSOM does not support removing hidden fields   

**Namespace:** [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md)  
**Assembly:** OfficeDevPnP.Core.dll  
## Syntax
```C#
public static void SetRating(this List list, VotingExperience experience)
```
### Parameters
#### list  
&emsp;&emsp;Type: Microsoft.SharePoint.Client.List  
&emsp;&emsp;Current List  

  

#### experience  
&emsp;&emsp;Type: [OfficeDevPnP.Core.VotingExperience](OfficeDevPnP.Core.VotingExperience.md)  
&emsp;&emsp;Likes/Ratings  

  

### Return Value
Type: void  

## See also
- [ListRatingExtensions](Microsoft.SharePoint.Client.ListRatingExtensions.md) 
- [Microsoft.SharePoint.Client](Microsoft.SharePoint.Client.md) 
