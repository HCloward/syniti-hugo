+++
title = 'Register Plugin in DSP®'
solution = 'Platform'
+++

# Register Plugin in DSP®

Once the plugin is created, it must be registered in the DSP.

To register a plugin in the DSP:

1.  [Create a user area folder](#CreateUserAreaFolder)
2.  [Register the plugin assembly](#RegisterPluginAssembly)
3.  [Access Back End Authentication](#AccessBackEndAuthentication)
4.  [Register the plugin as an external
    page](#RegisterPluginasanExternalPage)

## <span id="CreateUserAreaFolder"></span>Create User Area Folder

The User Area folder is a location for the plugin files on the
application server.  During the installation of the DSP, the base
UserArea folder will be created as follows: \[DSP Install
Directory\]/Web/UserArea/\[WebAppID\]. \[WebAppID\] is the GUID specific
to the WebApp.

To create a user area folder for the plugin:

1.  Locate or create a folder on the DSP server that is the same name as
    WebApp ID of the application to which the plugin is to be
    registered.

2.  Create a sub folder called “Processes”.

3.  Copy the plugin assembly DLL files into the Processes folder.

For example,

\[DSP Install
Directory\]/Web/UserArea/9AC95B56-F805-4FC4-0000-590B05CD0E7C/Processes/myassembly.dll

## <span id="RegisterPluginAssembly"></span>Register the Plugin Assembly

A plugin assembly is the deployment container of one or many plugins. In
the case of the DSP plugins, a plugin assembly is a DLL created using a
Microsoft .Net compiler (commonly Visual Studio). It is the plugin
assembly that is registered in DSP.

To register the plugin assembly:

1.  Select **Admin \> WebApps** in the *Navigation* pane.

2.  Click the **Plugins** icon for the desired WEB APP NAME.

3.  Click **Add**.
    
    [*View the field descriptions for the Plugin Assemblies
    page*](../Page_Desc/Plugin%20Assemblies%20H.htm)

4.  Enter the plugin assembly name in the **RELATIVE ASSEMBLY PATH**
    field.
    
    **NOTE:** The RELATIVE ASSEMBLY PATH field displays the plugin
    assembly name relative to the UserArea\\\[WebAppID\]\\Processes
    folder, where UserArea is the DSP folder on the application server
    where all assemblies are stored and WebAppID is the GUID specific to
    the WebApp. If the DLL is in the Processes folder, only the assembly
    name displays. If the DLL is in another folder or a sub-folder, the
    assembly name and the path display. For example, with an assembly
    called "myassembly.dll" located in the Processes folder, the
    Relatively Assembly Path displays "myassembly.dll." However, if that
    assembly was in a sub-folder called "bin," the Relative Assembly
    Path displays "bin\\myassembly.dill."

<!-- end list -->

1.  Click **Save**; all plugins within the plugin assembly are
    automatically registered to the DSP. The remaining fields are
    populated from the DLL.
2.  Click the **Plugins** icon to verify that all plugins were created.
    If plugins are missing:
      - Check the assembly to be sure the Plugin Installer attributes
        were sent and that the plugin classes are Public.
      - Ensure the correct DLL file is referenced in the Relative
        Assembly
Path.

## <span id="AccessBackEndAuthentication"></span>Access Back End Authentication

If configured to use Back End Authentication, when the Plugin is
executed from an event, the DSP prompts the user for Authentication
details (username and password) and stores these details for the current
session of the user. In order for these authentication details to be
accessed by the plugin, the following code and configuration must be
implemented to access Back End Authentication.

To access Back End Authentication:

1.  Add the **DependsOnExternalSystem(ExternalSystemType).SAP**
    attribute for C\#.
    
    OR
    
    Add the
    **DependsOnExternalSystem(RuntimeModel.ExternalSystemType.SAP)**
    attribute for Visual Basic .Net.
    
    **NOTE:** These attributes allow the DSP to access the UserName and
    Password via properties on the Session.

2.  Enter the Back End Authentication details to access the user name
    and password entered by users through the DSP’s Back End
    Authentication window. These details can be accessed from properties
    of the Host class.

3.  Enable Back End Authentication for the plugin. Refer to the [Enable
    Back End
    Authentication](View%20Where%20Plugin%20is%20Used.htm#EnableBackEndAuthentication)
    section for more
information.

## <span id="RegisterPluginasanExternalPage"></span>Register Plugin as an External Page

Once the plugin is registered to DSP, it must be registered to an event
as an external page.

To register the plugin as an external page:

1.  Select **Admin \> WebApps** in the *Navigation* pane.

2.  Click the **Pages** icon for the desired WEB APP NAME.

3.  Click the **Events** icon for the desired page DESCRIPTION.

4.  Click the **Business Rule**s icon for the desired EVENT.

5.  Click **Add**.
    
    [*View the field descriptions for the Page Business Rules
    page*](../Page_Desc/Page_Business_Rules_H.htm)

6.  Enter a value in the **Priority** field to determine the order the
    business rules run for the event.

7.  Select **External Page** from the **PROCEDURE TYPE** list box.

8.  Click **Save**; the *Vertical* View displays.
    
    [*View the field descriptions for the Page Business Rules page’s
    Vertical
    View*](../Page_Desc/Page_Business_Rules_H.htm#PageBusinessRulesV)

9.  Select the plugin from the **WebApp Plugin Type Code** list box.

10. Enter a brief description of the plugin in the **Comment** field.

11. Click **Save**.

**NOTE:** Additional fields can be configured for the external page.
Refer to the [Business Rules](../../WebApp_Dev/Business_Rules.htm) page
for more information.
