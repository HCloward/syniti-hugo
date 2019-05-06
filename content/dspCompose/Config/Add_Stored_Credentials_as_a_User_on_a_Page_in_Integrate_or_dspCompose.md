# Add Stored Credentials as a User on a Page in Integrate or dspCompose™

Credentials allow users to add and maintain their user name and password
for a data source where data is to be posted or where BDC and GUI
Scripts are recorded. Changes made to target system data can be tracked
to this user.

Before performing this task, the Template Administrator must add a
template. Refer to [Create a BDC Script
Template](../Use_Cases/Create_a_BDC_Script_Template.htm) and [Create a
GUI Script Template](../Use_Cases/Create_a_GUI_Script_Template.htm) in
dspCompose™ or [Manage
Templates](../../../Platform/Integrate/Use_Cases/Manage_Templates.htm)
in Integrate for more information.

The user credentials for the connection can be supplied using different
methods. Refer to [User Credentials in
dspCompose™](User_Credentials_in_dspCompose.htm) for more information.

In Integrate, a user can store credentials for BDC Script, GUI Script,
BAPI and RFC template types. In dspCompose™, credentials can be stored
for BDC scripts and GUI scripts.

<span style="font-weight: bold;">NOTE</span>: A user can add one set of
stored credentials for the user name per data source.  

<span style="font-weight: bold;">NOTE</span>: Credentials are required
when recording a BDC Script or GUI Script. If the system does not detect
credentials when the user clicks the Record icon on the
<span style="font-style: italic;">[Template](../../../Platform/Integrate/Page_Desc/Template_H.htm)</span>
page’s <span style="font-style: italic;">Vertical</span> View in
Integrate, or clicks the Record icon on the
<span style="font-style: italic;">[Create Template
(Recording)](../Use_Cases/Create_Template_Recording.htm)</span> page in
dspCompse™, the <span style="font-style: italic;">[User
Credentials](../../../Platform/Common/Page_Desc/User_Credentials_H.htm)</span>
page displays and the user must add credentials. Refer to [User
Credentials in dspCompose™](User_Credentials_in_dspCompose.htm) for more
information.  If credentials are detected, the recording process
continues as expected  

<span style="font-weight: bold;">NOTE</span>: The data source for the
template is associated with the connection selected in the CONNECTION ID
list box on the
<span style="font-style: italic;">[Template](../../../Platform/Integrate/Page_Desc/Template_H.htm)</span>
page’s <span style="font-style: italic;">Horizontal</span> View in
Integrate. In dspCompose™, the connection is selected on the
<span style="font-style: italic;">Vertical</span> View of the
<span style="font-style: italic;">[Templates](../Page_Desc/Templates_H.htm)</span>
page. When the connection is set, the data source for the template is
also set.

To add user credentials as a user in Integrate:

1.  Click <span style="font-weight: bold;">Categories</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Templates</span> icon for
    a category.

3.  Click <span style="font-weight: bold;">Vertical View</span> for a
    template of type BDC Script, GUI Script, BAPI or RFC.

4.  Click the <span style="font-weight: bold;">User Credentials</span>
    icon; <span style="font-style: italic;">Vertical</span> View
    displays.
    
    **NOTE:** If the source page specifies a specific connection, the
    <span style="font-style: italic;">[User
    Credentials](../../../Platform/Common/Page_Desc/User_Credentials_H.htm)</span>
    page's <span style="font-style: italic;">Vertical</span> View
    displays. If the source page does not have a specific connection,
    the <span style="font-style: italic;">Horizontal</span> View of the
    <span style="font-style: italic;">User Credentials</span> page
    displays, allowing a user to modify the credentials for various
    connections.

5.  Select a language in the <span style="font-weight: bold;">SAP
    Language</span> list box.

6.  Enter the user ID to the data source in the
    <span style="font-weight: bold;">SAP User ID</span> field.

7.  Enter the password associated with the user ID in the
    <span style="font-weight: bold;">SAP Password</span> field.

8.  Click <span style="font-weight: bold;">Save</span>.

To add user credentials as a user in dspCompose™:

1.  Click <span style="font-weight: bold;">Team</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Templates</span> icon for
    a team.

3.  Click <span style="font-weight: bold;">Vertical View</span> for a
    template.

4.  Click the <span style="font-weight: bold;">User Credentials</span>
    icon; <span style="font-style: italic;">Vertical</span> View
    displays.
    
    **NOTE:** If the source page specifies a specific connection, the
    <span style="font-style: italic;">[User
    Credentials](../../../Platform/Common/Page_Desc/User_Credentials_H.htm)</span>
    page's <span style="font-style: italic;">Vertical</span> View
    displays. If the source page does not have a specific connection,
    the <span style="font-style: italic;">Horizontal</span> View of the
    <span style="font-style: italic;">User Credentials</span> page
    displays, allowing a user to modify the credentials for various
    connections.

5.  Select a language in the <span style="font-weight: bold;">SAP
    Language</span> list box.

6.  Enter the user ID to the data source in the
    <span style="font-weight: bold;">SAP User ID</span> field.

7.  Enter the password associated with the user ID the
    <span style="font-weight: bold;">SAP Password</span> field.

8.  Click <span style="font-weight: bold;">Save</span>.

9.  Click the <span style="font-weight: bold;">Test Connection</span>
    icon in the Page toolbar to confirm that a connection to the target
    system can be established using the user credentials.
