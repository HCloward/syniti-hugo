+++
title = 'Set the Auto Gen Level for a Target'
solution = 'Migration'
+++

# Set the Auto Gen Level for a Target

A setting on the
<span style="font-style: italic;">[Automation](../Page_Desc/Automation_page.htm#Automation_V)</span>
page’s <span style="font-style: italic;">Vertical</span> View configures
if and how SQL Objects are auto-generated in the database and registered
in Transform.

<span style="font-weight: bold;">NOTE:</span> Altered table commands are
used to add missing columns. Rules only create views and stored
procedures that are missing. They do not update any views or stored
procedures.

The Auto Gen Levels are:

  - **New Rules – Alter Table and Build New Views and Stored Procedures
    Only –** When autogenerating, a table is updated and only new views
    and stored procedures are created. Existing views and stored
    procedures are not updated.

  - **Off – No Generating Any SQL Objects –** AutoGen is not used.
    
    **NOTE:** Rules for mappings with the Copy, Default, Rule, XRef, and
    Xref actions are not built. For mappings with the Construction
    action (for example, mappings that use Enhanced Construction), the
    table and field are not created in the target database and a page is
    not created in Construct. Full Construction objects are built via
    the Sync in Target Design. The rules must be generated on the
    <span style="font-style: italic;">[Automation SQL Field
    Mappings](../Page_Desc/Automation_SQL_Field_Mappings_H.htm)</span>
    page. Refer to [Create Rules](Create_Rules.htm) for more
    information.

  - **On – Drop & Rebuild Table, Views and Stored Procedures –** Any SQL
    objects previously created for the target are dropped and a new
    table, SQL views and stored procedures with the same name are added.

  - **Rebuild – Alter Table and Drop & Rebuild Views And Stored
    Procedures –** The table is updated. Views and stored procedures
    previously created for the target are dropped and new SQL views and
    stored procedures with the same name are added.

To set the Auto Gen Level for a Target in AutoGen:

1.  Click the **Automation** tab in the Quick Panel.

2.  Click the <span style="font-weight: bold;">Vertical View</span> icon
    for an Object.

3.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Automation page’s Vertical
    View.](../Page_Desc/Automation_page.htm#Automation_V)

4.  Select an option in the <span style="font-weight: bold;">Auto Gen
    Level</span> list box.

5.  Click <span style="font-weight: bold;">Save</span>.
