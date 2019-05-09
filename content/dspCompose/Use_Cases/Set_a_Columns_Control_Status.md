+++
title = 'Set a Column’s Control Status'
solution = 'Data Quality'
+++

# Set a Column’s Control Status

A Template Administrator can designate which columns display on a
template for each Review role. The Control Status for a column in a
template can be set to Enabled, Disabled, or Hidden at the
template-Review role level.

**NOTE**: Control Status for columns can only be used for
dspCompose™-generated pages and is not available for custom pages.

**NOTE:** This feature works in conjunction with column properties set
at the page level in the platform. dspCompose™ uses the most restrictive
setting when displaying columns. In general, the Hidden setting for a
column is more restrictive then a Disabled setting, and a Disabled
setting is more restrictive than an Enabled setting. For example, if a
column is hidden at the page level in the platform but is enabled at the
template-Review role level in dspCompose™, the column will be hidden.

**NOTE:** On the *Template (Role*) page, the **Columns** and **Excel
Column Control** icons are disabled after a user records a template.
Once the template is generated, these icons are enabled. To generate a
template, on the *Templates* page’s *Vertical* View, click **Generate**.

**NOTE:** If the user creates a template with roles that have custom
pages assigned, the **Columns** icon on the *Template (Role)* page is
disabled for those roles with custom pages even after the template is
generated.

**NOTE:** To change these settings, the template must not be active or
must be in Developer Mode. Refer to [Modify an Active Template in
Developer Mode](Modify_an_Active_Template_in_Developer_Mode) for
more information.

To set a column’s Control Status for a template at the Review role
level:

1.  Click **Team** in the *Navigation* pane.

2.  Click **Templates** for a team.

3.  Click **Roles** for a template.

4.  Click **Columns** for the Review role.

5.  Click an icon on the Page toolbar to indicate the control status for
    the role for the selected column(s). Options are:
    
    <span style="font-weight: bold;">Enabled</span> - The column(s)
    display on the generated Excel file and can be viewed and edited for
    data entry.
    
    <span style="font-weight: bold;">Disabled</span> – The column(s)
    display on the generated Excel file and can be viewed but not edited
    for data entry.
    
    <span style="font-weight: bold;">Hidden</span> - The column(s) do
    not display on the generated Excel file.

<span style="font-weight: bold;">NOTE:</span> To select a contiguous
range of items, hold down the Shift key and select the first and last
items in the range. To select a noncontiguous range of items, hold down
the Ctrl key and select each item.

Refer to [Import a File at the Request-Role
Level](Import_a_File_at_the_Request%20Role_Level) for more
information.
