+++
title = 'Add List Boxes to an Excel File'
solution = 'Data Quality'
+++

# Add List Boxes to an Excel File

The Template Administrator can format the columns on the template’s
dspCompose-generated Excel file used for data entry. When the column’s
**Type** is set to **List Box**, the column on the Excel file will be
created with a list box.

List box values are configurable, based on a data source and values
selected by the Template Administrator.

List box values in Excel display based on the UserID and SAP Language of
the current user, if the boaUser ID and the boaSAPLanguage columns have
been added to the list view.

**NOTE**:To change the Excel Column Control settings for a template
role, the template must not be active or must be in Developer Mode.
Refer to [Modify an Active Template in Developer
Mode](Modify_an_Active_Template_in_Developer_Mode) for more
information.

**NOTE**:On the *Template (Role Excel Column Control)* page, the **Excel
Column Control** icon is disabled after a user records a template. Once
the template is generated, this icon is enabled. To generate a template,
on the *Template* page’s *Vertical* View, click **Generate**.

To add a list box to an Excel column:

1.  Click **Team** on *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Roles** for a template.

4.  Click **Excel Column Control** for a role.
    
    <span style="font-weight: bold;">NOTE</span>: This option is not
    available for the Post role.
    
    **NOTE**: The **TYPE** displays as Text Box on the
    <span style="font-style: italic;">Horizontal</span> View until the
    list setting are configured.

5.  Click **Vertical View** for a column.

6.  Click **Edit**.
    
    *[View the field descriptions for the Template (Role Excel Column
    Control) page’s Vertical
    View.](../Page_Desc/Template_Role_Excel_Column_Control_H)*

7.  Select the data source for the list box values in the **List Data
    Source ID** list box.
    
    **NOTE:** The List Data Source ID is the data source that contains
    the view or table used in a list box.

8.  Select the source for the list box values from the **List Source**
    list box.
    
    **NOTE:** The List Source is the view or table that contains the
    values used in a list box.

9.  Select the list value from the **List Value** list box.
    
    **NOTE:** The List Value is the column that contains the value used
    within a list box.

10. Select the list display in the **List Display** list box.
    
    **NOTE**: The List Display is what will display for the user in the
    list box in the Excel file. This value is ignored on import.

11. Click **Save**.

**NOTE**:  The row for this column displays **List Box** in the **TYPE**
column on the <span style="font-style: italic;">Horizontal</span> View.

**NOTE**: When the Template Administrator clicks the **Import Column**
button on the *Template (Role Excel Column Control)* page, dspCompose
imports all list boxes from the assigned platform page. Once the list
box settings are imported from the platform, the Template Administrator
should verify that these list box settings (source, value column,
display column) are valid in Excel. Refer to [Import a Column Added to
the Role’s Assigned
Page](Import_a_Column_Added_to_the_Roles_Assigned_Page) for more
information.
