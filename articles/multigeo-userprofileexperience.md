# User profiles in a SharePoint Multi-Geo tenant

> **Important:** OneDrive and SharePoint Online Multi-Geo is currently in preview and is subject to change.

In a Multi-Geo tenant, you can define a preferred data location for a user. This article also describes how to find a user's OneDrive site and how to read and update default and custom user profile properties.

## Where are user profiles located in a Multi-Geo tenant?
In a Multi-Geo tenant, SharePoint users span the different geo locations - for example, some users are in North America, some in Europe, and so on. This model also applies to user accounts and personal sites (OneDrive for Business sites). Ideally, the users and their user accounts and sites are in the same geo location. To ensure this, before you create personal sites, you set the user's preferred data location to their geo location. 

As shown in the following image, user vesa@contoso.onmicrosoft.com is living in Europe and has a preferred data location set to **EUR**. As such:
 
- The default copy of the user's profile is in the Europe geo location.
- The user's personal site is created in the Europe geo location.

User bert@contoso.onmicrosoft.com has his preferred data location set to **NAM**. Because he already had a personal site hosted in Europe before his preferred data location was set, his profile stays in Europe. 

![World map showing default geo location in North America and satellite locations in Europe and Asia, with users, geo locations, and preferred data locations set](media/multigeo/multigeouserprofiles_intro.png)

Users' profile and personal sites are in the same geo location. For users who do not have a personal site:

- If the user has a preferred data location set, their profile is located in that geo location.
- If the user does not have a preferred data location set, their profile is located in the default geo location.

To programmatically discover the user's profile location, you can do one of the following:

- Use the SharePoint User Profile API. We recommend this approach because it works in all scenarios. 
- Use the Microsoft Graph. This works for users who also have personal sites, but not for users who don't have personal sites.

### Use the SharePoint User Profile API to detect the profile location
The SharePoint user profile API, which can be called via either REST or CSOM, allows you to retrieve the personal site host URL for a given account. This personal site host URL will contain the personal site host for the user's personal site, Regardless of whether this personal site has been created. The following example shows the REST call.

```
GET https://contoso.sharepoint.com/_api/SP.UserProfiles.PeopleManager/GetPropertiesFor(accountName=@v)/personalsitehosturl?%40v=%27i%3A0%23.f%7Cmembership%7Cbert%40contoso.onmicrosoft.com%27
```

If you're using C#, CSOM, as shown in the following example, is easier to use.

```C#
public string GetUserPersonalSiteHostUrlCSOM(ClientContext ctx, string userPrincipalName)
{
    string result = null;

    PeopleManager peopleManager = new PeopleManager(ctx);
    var userProperties = peopleManager.GetPropertiesFor(userPrincipalName);
    this.clientContext.ExecuteQuery();
    result = userProperties.PersonalSiteHostUrl;

    return result;
}
```

Once you have the personal site host url you can use that to cross it with the Multi-Geo discovery information (see the [Multi-Geo Discovery](multigeo-discovery.md) article) to get the tenant admin site url for the geo location hosting the user's profile.

To learn more, see the [MultiGeo.UserProfileUpdates](https://github.com/SharePoint/PnP/tree/dev/Samples/MultiGeo.UserProfileUpdates) sample.

### Use Microsoft Graph to detect the user's personal site url
Discovering a user's personal site is an important task in a multi geo tenant: if you want to update the user's profile knowing the personal site url will tell you where the profile lives. The recommended method for getting the user's personal site url is using the following Microsoft Graph call:

```
GET https://graph.microsoft.com/v1.0/users/bert@contoso.onmicrosoft.com?$select=mySite
```

Once you have the personal site url you can cross that with the Multi-Geo discovery information (see the [Multi-Geo Discovery](multigeo-discovery.md) article) to get the tenant admin site url for the geo location hosting the user's profile. 

>**Note:**
>In case the user does not have a personal site yet this approach will not help you detect where the user's profile lives. Refer to the SharePoint User Profile API described in previous chapter in that case.

To learn more, see the [MultiGeo.UserProfileUpdates](https://github.com/SharePoint/PnP/tree/dev/Samples/MultiGeo.UserProfileUpdates) sample.

## Manipulating user profile properties
A common scenario, especially for enterprise customers, is performing bulk updates of user profile properties. Depending on the type of user profile property you'll need to use a different approach as explained in below chapters.

### Out-of-the-box user profile properties
Out of the box user profile properties are properties which are available by default. Samples are for example the Department, AboutMe, PreferredDataLocation...and many more. The recommended model for manipulating these properties is using the Microsoft Graph API: when using the Microsoft Graph API you don't need to be aware of the geo location of the profile, the Microsoft Graph API will handle this for you.

```
GET https://graph.microsoft.com/v1.0/users/bert@contoso.onmicrosoft.com?$select=aboutme
```

To learn more, see the [MultiGeo.UserProfileUpdates](https://github.com/SharePoint/PnP/tree/dev/Samples/MultiGeo.UserProfileUpdates) sample.

#### What about the user's preferred data location (preferredDataLocation) property?
The user's preferred data location (preferredDataLocation) is special kind of property: this property indicates the preferred geo location of this user which impacts the following:
- The user's personal site will be provisioned in this geo location
- When that user creates a "modern" team site (a.k.a. group site) then this site will be created in this geo location

Since the preferred data location is an out of the box property the recommended approach to configure it is using the Microsoft Graph API. 

```
GET https://graph.microsoft.com/v1.0/users/bert@contoso.onmicrosoft.com?$select=preferredDataLocation

PATCH https://graph.microsoft.com/beta/users/bert@contoso.onmicrosoft.com

JSON payload:
{
    "preferredDataLocation" : "eur"
}

```

To learn more, see the [MultiGeo.UserPreferredDataLocation](https://github.com/SharePoint/PnP/tree/dev/Samples/MultiGeo.UserPreferredDataLocation) sample.

### Custom created SharePoint specific user profile properties
Customers often have a need to add company specific user profile properties, which is something that's possible for SharePoint user profiles. When working in a Multi-Geo tenant you need to take in account the following key considerations when you're working with custom user profile properties:
- Custom user profile properties are created at geo location level: so if you create a property in the Europe geo location then that property is not available in the other geo locations. **It's a best practice to create custom user profile properties in all geo locations: this way there's no risk on data loss when a user is moved across geo locations**.
- Reading and updating custom user profile properties will need to be done at geo location level: if you've a custom property in all geo locations then you need you would need to iterate over the geo regions and update the property for the users having their profile in the geo region.

```C#
// For SPO custom created properties use below approach
string userPrincipalName = "bert@contoso.onmicrosoft.com";
string userAccountName = $"i:0#.f|membership|{userPrincipalName}";
PeopleManager peopleManager = new PeopleManager(tenantAdminContext);
var propsToRetrieve = new string[] { "CostCenter", "CustomProperty" };
var props = peopleManager.GetUserProfilePropertiesFor(new UserProfilePropertiesForUser(tenantAdminContext, userAccountName, propsToRetrieve));
tenantAdminContext.ExecuteQuery();

int i = 0;
foreach (var prop in props)
{
    Console.WriteLine($"Prop: {propsToRetrieve[i]} Value: {prop}");
    i++;
}

// Update user profile properties
peopleManager.SetSingleValueProfileProperty(userAccountName, "CostCenter", "89786879");
tenantAdminContext.ExecuteQuery();
```

To learn more, see the [MultiGeo.UserProfileUpdates](https://github.com/SharePoint/PnP/tree/dev/Samples/MultiGeo.UserProfileUpdates) sample.

#### Can I still use the batch user profile update API
The [bulk user profile update API](https://msdn.microsoft.com/en-us/pnp_articles/bulk-user-profile-update-api-for-sharepoint-online) is specifically designed to perform mass updates on custom user profile properties and can still be used in a Multi-Geo tenant taking in account the following considerations:
- This API works at geo location level and is not Multi-Geo aware: when you for example use the API in the Europe geo location then only accounts living in the Europe geo location can be updated
- If you specify an import file with accounts living in different geo locations then the bulk update API will only update the properties for the users that live in the same geo location as the geo location in which you submitted the import file


## Resources
Below list of resources are useful when you're learning more about working with user profiles in SharePoint Online:
- [Bulk user profile import documentation](https://msdn.microsoft.com/en-us/pnp_articles/bulk-user-profile-update-api-for-sharepoint-online)
- [Sample on using the batch user profile update API](https://github.com/SharePoint/PnP/tree/master/Samples/UserProfile.BatchUpdate.API)


