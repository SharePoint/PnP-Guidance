# Customizing modern lists and libraries
During summer 2016 the SharePoint Online team released "modern" document libraries and lists which brings a better user experience which is faster, more intuitive and responsive. This article focuses on the extensibility options there are in the "modern" library and list experiences, if you however want to learn more about the functionalities offered by the "modern" experiences then following links will help:
- Overview of the "modern" document library experience: https://blogs.office.com/2016/06/07/modern-document-libraries-in-sharepoint
- Overview of the "modern" list experience: https://blogs.office.com/2016/07/25/modern-sharepoint-lists-are-here-including-integration-with-microsoft-flow-and-powerapps 
- Differences between "modern" and "classic" experiences: https://support.office.com/en-us/article/Differences-between-classic-and-new-experiences-for-lists-and-document-libraries-30e1aab0-a5cc-4363-b7f2-09e2ae07d4dc?ui=en-US&rs=en-US&ad=US

In remainder of this article we'll use "modern" for the new user experience and "classic" for the legacy user experience. 

>**Important:** 
We're not deprecating the "classic" experience, both "classic" and "modern" will coexist.


_**Applies to:** SharePoint Online_

## Overview of the customization options
Below table gives a quick overview of the supportability of "modern" lists and libraries, in this article we'll provide more details and examples on the supported options. The SharePoint team is working to support more options in the future.

| **Not Supported** | **Supported options** |
|:-----|:-----|
| JSLink based field customizations| Subset of User Custom Actions  |
| JSLink based view customizations | Custom branding  |
| Custom CSS via AlternateCSSUrl web property |  |
| Custom JavaScript embedded via User Custom Actions |  |
| Custom master pages |  |
| Customization via InfoPath |  |
| Minimal Download Strategy (MDS) |  |
| SharePoint Server Publishing |  |


## User Custom Actions
<a name="supportedcustomactions"> </a>
The "modern" experiences do allow certain user custom actions to be surfaced in the new user interface, but not all user action configurations which are supported by "classic" mode are supported in the "modern" experience. Below table gives a high level overview of the supported custom action locations and how they're surfaced in the "modern" UI:

|**User Custom Action location**|**Visible in "modern" UI**|
|:-----|:-----|
| `EditControlBlock` | Yes, these entries show up as custom menu items|
| `CommandUI.Ribbon` | Yes, these entries show up as toolbar items |
| All other locations (e.g. `scriptlink`) | Sorry, these user custom actions won't work |


### EditControlBlock User Custom Actions 
<a name="editcontrolblockcustomactions"> </a>
Adding custom links to the context menu can be done by using the `EditControlBlock` as location for your custom action. The below PnP provisioning XML creates 2 custom entries. 

```XML
<pnp:ProvisioningTemplate ID="EditControlBlockSamples" Version="1" xmlns:pnp="http://schemas.dev.office.com/PnP/2015/12/ProvisioningSchema">
  <pnp:CustomActions>
    <pnp:SiteCustomActions>
      <pnp:CustomAction Name="CA_1" Description="ca 1" Location="EditControlBlock" RegistrationType="List" RegistrationId="101" Title="CA 1 Title" Sequence="3000" Url="https://contoso.azurewebsites.net/pages/index.aspx" Enabled="true"/>
      <pnp:CustomAction Name="CA_2" Description="ca 2" Location="EditControlBlock" RegistrationType="List" RegistrationId="101" Title="CA 2 Title" Sequence="4000" Url="https://contoso.azurewebsites.net/pages/index.aspx" Enabled="true"/>
    </pnp:SiteCustomActions>
  </pnp:CustomActions>
</pnp:ProvisioningTemplate>
```

You can apply this PnP provisioning template to a site using the PnP Core library or PnP PowerShell. We've opted to show the PowerShell approach in this article. A first step is installing the PnP PowerShell module as described in https://github.com/SharePoint/PnP-PowerShell. Once that's done, save the PnP provisioning xml to a file and then 2 simple lines of PnP PowerShell are enough to apply the template:

```PowerShell
Connect-PnPOnline -Url <url_to_your_SharePoint_Online_site>
Apply-PnPProvisioningTemplate -Path c:\customaction_modern_editcontrolblock.xml -Handlers CustomActions
```

If you refresh the "modern" view of a document library in your site you'll see the new entries appear

![EditControlBlock actions](http://i.imgur.com/ELrG5Sb.png)


>**Note**:
>If you want to use this sample for a list then please set the `RegistrationId` attribute to 100

### CommandUI.Ribbon User Custom Actions 
<a name="ribboncustomactions"> </a>
If you want to extend the toolbar in the "modern" list and library experiences you can do so via adding a user custom action targeting the CommandUI.Ribbon location as shown in the PnP provisioning XML sample

```XML
<pnp:ProvisioningTemplate ID="CommandUIRibbonSamples" Version="1" xmlns:pnp="http://schemas.dev.office.com/PnP/2015/12/ProvisioningSchema">
  <pnp:CustomActions>
    <pnp:SiteCustomActions>
      <pnp:CustomAction Name="CA_4" Description="ca 4" Location="CommandUI.Ribbon" RegistrationType="List" RegistrationId="101" Title="CA 4 Title" Sequence="6000" Enabled="true">
        <pnp:CommandUIExtension>
          <CommandUIDefinitions>
            <CommandUIDefinition Location="Ribbon.Documents.Copies.Controls._children">
              <Button
                Id="Ribbon.Documents.Copies.OfficeDevPnPDownloadAll"
                Command="OfficeDevPnP.Cmd.DownloadAll"
                Image16by16="/_layouts/15/images/sharepointfoundation16.png"
                LabelText="Download All"
                Description="Download all files separately"
                ToolTipTitle="Download All"
                ToolTipDescription="Download all files separately"
                TemplateAlias="o1"
                Sequence="15"/>
            </CommandUIDefinition>
          </CommandUIDefinitions>
          <CommandUIHandlers>
            <CommandUIHandler
              Command="OfficeDevPnP.Cmd.DownloadAll"
              CommandAction="https://contoso.azurewebsites.net/pages/index.aspx" />
          </CommandUIHandlers>
        </pnp:CommandUIExtension>
      </pnp:CustomAction>
      <pnp:CustomAction Name="CA_6" Description="ca 6" Location="CommandUI.Ribbon" RegistrationType="List" RegistrationId="101" Title="CA 6 Title" Sequence="5000" Enabled="true">
        <pnp:CommandUIExtension>
            <CommandUIDefinitions>
              <CommandUIDefinition Location="Ribbon.CustomTabs._children">
                <Tab Id="Custom Tab" Title="Custom Tab" Description="Custom Tab">
                  <Scaling Id="Custom Tab.Scaling">
                    <MaxSize Id="Custom Group.Scaling.MaxSize" GroupId="Custom Group" Size="LargeLarge" />
                    <MaxSize Id="Custom Group 2.Scaling.MaxSize" GroupId="Custom Group 2" Size="LargeLarge" />
                    <Scale Id="Custom Group.Scaling.Scale" GroupId="Custom Group" Size="LargeLarge" />
                    <Scale Id="Custom Group 2.Scaling.Scale" GroupId="Custom Group 2" Size="LargeLarge" />
                  </Scaling>
                  <Groups Id="Custom Tab.Groups">
                    <Group Id="Custom Group 2" Title="Custom Group 2" Description="Custom Group 2" Sequence="7888" Template="Ribbon.Templates.Flexible2">
                      <Controls Id="Custom Group 2.Controls">
                        <Button Id="CustomButton3" LabelText="Custom Button 3" Image16by16="/_layouts/15/images/attach16.png" ToolTipTitle="Custom Button 3" ToolTipDescription="Custom Button 3" Command="CustomButton3.Command" TemplateAlias="o1" />
                      </Controls>
                    </Group>
                    <Group Id="Custom Group 1" Title="Custom Group 1" Description="Custom Group 1" Sequence="10000" Template="Ribbon.Templates.Flexible2">
                      <Controls Id="Custom Group 1.Controls">
                        <Button Id="CustomButton1" LabelText="Custom Button 1" Image16by16="/_layouts/15/images/itslidelibrary.png" ToolTipTitle="Custom Button 1" ToolTipDescription="Custom Button 1" Command="CustomButton1.Command" TemplateAlias="o1" />
                        <Button Id="CustomButton2" LabelText="Custom Button 2" Image16by16="/_layouts/15/images/dldsln16.png" ToolTipTitle="Custom Button 2" ToolTipDescription="Custom Button 2" Command="CustomButton2.Command" TemplateAlias="o1" />
                      </Controls>
                    </Group>
                  </Groups>
                </Tab>
              </CommandUIDefinition>
              <CommandUIDefinition Location="Ribbon.Templates._children">
                <GroupTemplate Id="Ribbon.Templates.Flexible2">
                  <Layout Title="LargeLarge" LayoutTitle="LargeLarge">
                    <OverflowSection DisplayMode="Large" TemplateAlias="o1" Type="OneRow" />
                    <OverflowSection DisplayMode="Large" TemplateAlias="o2" Type="OneRow" />
                  </Layout>
                  <Layout Title="LargeMedium" LayoutTitle="LargeMedium">
                    <OverflowSection DisplayMode="Large" TemplateAlias="o1" Type="OneRow" />
                    <OverflowSection DisplayMode="Medium" TemplateAlias="o2" Type="ThreeRow" />
                  </Layout>
                  <Layout Title="LargeSmall" LayoutTitle="LargeSmall">
                    <OverflowSection DisplayMode="Large" TemplateAlias="o1" Type="OneRow" />
                    <OverflowSection DisplayMode="Small" TemplateAlias="o2" Type="ThreeRow" />
                  </Layout>
                  <Layout Title="MediumLarge" LayoutTitle="MediumLarge">
                    <OverflowSection DisplayMode="Medium" TemplateAlias="o1" Type="ThreeRow" />
                    <OverflowSection DisplayMode="Large" TemplateAlias="o2" Type="OneRow" />
                  </Layout>
                  <Layout Title="MediumMedium" LayoutTitle="MediumMedium">
                    <OverflowSection DisplayMode="Medium" TemplateAlias="o1" Type="ThreeRow" />
                    <OverflowSection DisplayMode="Medium" TemplateAlias="o2" Type="ThreeRow" />
                  </Layout>
                  <Layout Title="MediumSmall" LayoutTitle="MediumSmall">
                    <OverflowSection DisplayMode="Medium" TemplateAlias="o1" Type="ThreeRow" />
                    <OverflowSection DisplayMode="Small" TemplateAlias="o2" Type="ThreeRow" />
                  </Layout>
                  <Layout Title="SmallLarge" LayoutTitle="SmallLarge">
                    <OverflowSection DisplayMode="Small" TemplateAlias="o1" Type="ThreeRow" />
                    <OverflowSection DisplayMode="Large" TemplateAlias="o2" Type="OneRow" />
                  </Layout>
                  <Layout Title="SmallMedium" LayoutTitle="SmallMedium">
                    <OverflowSection DisplayMode="Small" TemplateAlias="o1" Type="ThreeRow" />
                    <OverflowSection DisplayMode="Medium" TemplateAlias="o2" Type="ThreeRow" />
                  </Layout>
                  <Layout Title="SmallSmall" LayoutTitle="SmallSmall">
                    <OverflowSection DisplayMode="Small" TemplateAlias="o1" Type="ThreeRow" />
                    <OverflowSection DisplayMode="Small" TemplateAlias="o2" Type="ThreeRow" />
                  </Layout>
                </GroupTemplate>
              </CommandUIDefinition>
            </CommandUIDefinitions>
            <CommandUIHandlers>
              <CommandUIHandler Command="CustomButton1.Command" CommandAction="https://contoso.azurewebsites.net/pages/index.aspx" />
              <CommandUIHandler Command="CustomButton2.Command" CommandAction="http://www.bing.com" />
              <CommandUIHandler Command="CustomButton3.Command" CommandAction="http://dev.office.com/sharepoint" />
            </CommandUIHandlers>
        </pnp:CommandUIExtension>
      </pnp:CustomAction>
    </pnp:SiteCustomActions>
  </pnp:CustomActions>
</pnp:ProvisioningTemplate>
```

After adding these user custom actions you'll see them appearing in the toolbar. Notice that custom tabs are transformed into a dropdown menu:

![](http://i.imgur.com/fb9pQqD.png)

>**Note**:
>If you want to use this sample for a list then please set the `RegistrationId` attributes to 100 and use the below XML for the CA_4 user custom action
>
```XML
<CommandUIDefinition Location="Ribbon.Templates._children">
  <Button
    Id="Ribbon.Templates.OfficeDevPnPDownloadAll"
    Command="OfficeDevPnP.Cmd.DownloadAll"
    Image16by16="/_layouts/15/images/sharepointfoundation16.png"
    LabelText="Download All"
    Description="Download all files separately"
    ToolTipTitle="Download All"
    ToolTipDescription="Download all files separately"
    TemplateAlias="o1"
    Sequence="15"/>
</CommandUIDefinition>
```

### User Custom Action limitations 
<a name="customactionlimitations"> </a>

When developing user custom actions that need to work in modern experiences please take in account the following limitations:
 - You can't completely control the order in which the user custom actions show up: the user custom actions are added in the order the `_api/web/Lists(guid'listid')/CustomActionElements` does return the user custom actions...and this API currently does not take in account the sequence attributes. Buttons defined inside a custom tab can be ordered by adding them in the correct order in the CommandUIDefinition xml. Our sample shows Button 3 as first and that's because of the order in the XML
 - Command actions cannot contain JavaScript...using for example `CommandAction="javascript:alert('My custom Action');"` will mean the user custom action will not show up
 - Using the `ScriptLink` or `ScriptBlock` properties is not possible since they can only be used with user custom action location `ScriptLink`, which is not supported
 - The `RegistrationId` cannot refer to specific library ID (e.g. {7A46F86F-D6CC-4263-8A1B-1BC1658B506C}) or a specific content type id (e.g. 0x0101), only out of the box template types (e.g. 100 for a List or 101 for a Document Library) are allowed
 - Using image maps (e.g. `Image16by16="/_layouts/15/1033/images/formatmap16x16.png?rev=33" Image16by16Left="-144" Image16by16Top="-107"`) does not work, you'll need to specify individual images. Also note that only 16x16 images are relevant


## Custom branding
<a name="themingimpact"> </a>
If you're site happens to use a custom theme then this custom theme will be respected in the "modern" list and library experiences as shown in below sample:

![](http://i.imgur.com/jSzKsvo.png)

## How to configure the end user experience
<a name="configuremodernlibrariesandlists"> </a>
You do have multiple options to control whether the "modern" or "classic" library and list experience will be used. 

### Tenant level configuration
If you completely want to disable the "modern" experience then it's best to use the tenant setting for this. navigate to your tenant admin center (e.g. contoso-admin.sharepoint.com), go to settings and select the "classic" experience:

![](http://i.imgur.com/VlqKDh7.png)

### Site/Web level configuration
You can prevent a site collection or web to use the "modern" experience by enabling a feature:
- Site collection scoped feature with ID **E3540C7D-6BEA-403C-A224-1A12EAFEE4C4** for site collection control
- Web scoped feature with ID **52E14B6F-B1BB-4969-B89B-C4FAA56745EF** for web scoped control

You can use below PnP provisioning XML to enable this feature on site or web level

```XML
<pnp:ProvisioningTemplate ID="experiencecontrol" Version="1" xmlns:pnp="http://schemas.dev.office.com/PnP/2015/12/ProvisioningSchema">
  <pnp:Features>
    <!-- for site collection scoped control -->
    <pnp:SiteFeatures>
      <pnp:Feature ID="E3540C7D-6BEA-403C-A224-1A12EAFEE4C4" Description="Disable modern list experience"/>
    </pnp:SiteFeatures>
    <!-- for web scoped control -->
    <pnp:WebFeatures>
      <pnp:Feature ID="52E14B6F-B1BB-4969-B89B-C4FAA56745EF" Description="Disable modern list experience"/>
    </pnp:WebFeatures>
  </pnp:Features>
</pnp:ProvisioningTemplate>
```

Use following PnP PowerShell to apply this template:

```PowerShell
Connect-PnPOnline -Url <url_to_your_SharePoint_Online_site>
Apply-PnPProvisioningTemplate -Path c:\experiencecontrol.xml -Handlers Features
```

### List/Library configuration
If you want to control the experience on library level then you can use go to list settings, advanced settings and change the behavior:

![](http://i.imgur.com/Uebb6AV.png)

The same can also be done using CSOM as shown in below snippet:

```C#
var list = context.Web.Lists.GetByTitle(title);
context.Load(list);
context.ExecuteQuery();

list.ListExperienceOptions = ListExperience.ClassicExperience;

list.Update();
context.ExecuteQuery();
```

>**Note**:
> - The settings at library level override the settings at web, site or tenant level
> - The current configuration is cached, so changes are not immediately visible


## Additional resources
<a name="bk_addresources"> </a>

-  [Switch the default experience for lists or document libraries from new or classic](https://support.office.com/en-us/article/Switch-the-default-experience-for-lists-or-document-libraries-from-new-or-classic-66dac24b-4177-4775-bf50-3d267318caa9)
- [Overview of the "modern" document library experience](https://blogs.office.com/2016/06/07/modern-document-libraries-in-sharepoint)
- [Overview of the "modern" list experience](https://blogs.office.com/2016/07/25/modern-sharepoint-lists-are-here-including-integration-with-microsoft-flow-and-powerapps) 
- [Differences between "modern" and "classic" experiences](https://support.office.com/en-us/article/Differences-between-classic-and-new-experiences-for-lists-and-document-libraries-30e1aab0-a5cc-4363-b7f2-09e2ae07d4dc?ui=en-US&rs=en-US&ad=US)
