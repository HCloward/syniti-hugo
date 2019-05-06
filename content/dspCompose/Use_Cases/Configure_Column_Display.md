# Configure Column Display

At the template role level, a Template Administrator can control which
columns display in the generated data entry spreadsheet and on the
<span style="font-style: italic;">Data Entry</span> or the
<span style="font-style: italic;">Mass Changes</span> pages for a
request based on the template. <span>Whether a user can edit the data in
a column</span>  and column  color settings can also be configured.

Column display can be affected by settings:

  - At the template role level on the *Template (Role Excel Column
    Control)* page

  - At the template role level on the *Template (Role Column)* page

  - At the Review filter level if the role is Review

  - On the *Mass Change Exclude Columns* page

Refer to [Create Review
Filters](Add_Users_to_Templates.htm#Create_Review_Filters) and
[Configure Columns to Exclude from Mass
Change](../Config/Configure_Columns_to_Exclude_from_Mass_Change.htm) for
more information.

If multiple column display settings exist, dspCompose™ compares them and
uses the most restrictive column control status (set on the *Template
(Role Column)* page) to determine if a column should be displayed.
Hidden is more restrictive then Disabled. Disabled is more restrictive
then Enabled. Refer to [Set a Column’s Control
Status](Set_a_Columns_Control_Status.htm) for more information.

The *Template (Role Excel Column Control)* page allows the Template
Administrator to set:

  - Whether a column is included or excluded in the Excel file generated
    for data entry and on the data entry pages

  - Whether a column is read only

  - What type of control, such as a text box, is used to enter data

The <span style="font-weight: bold;">*Vertical* View</span> of the
*Template (Role Excel Column Control)* page allows the user to configure
further settings, such as colors, list settings, and custom validations.

**NOTE**: To configure template settings, the template must not be
active or must be in Developer Mode. Refer to [Modify an Active Template
in Developer Mode](Modify_an_Active_Template_in_Developer_Mode.htm) for
more information.

**NOTE**: On the *Template (Role*) page, the **Columns** and **Excel
Column Control** icons are disabled after a user records a template.
Once the template is generated, these icons are enabled. To generate a
template, on the *Template* page’s *Vertical* View, click **Generate**.

**NOTE**: For roles with custom pages, no columns are available for
editing on the *Template (Role Column)* page.

**NOTE**: Column display may be affected by additional settings.

To set column display on the *Template (Role Excel Column Control)*
page:

1.  Click **Team** on *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Roles** for a template.

4.  Click **Excel Column Control** for a role.
    
    **NOTE:** This icon is not active for the Post role.

5.  Select the record and click **Include** to include the column in the
    generated Excel file and on the
    <span style="font-style: italic;">Data Entry</span> and the
    <span style="font-style: italic;">Mass Change</span> pages.
    
    **NOTE:** When a user imports data from the Excel file to a request,
    this column’s display on the mapped page may be affected by
    additional settings in dspCompose™.
    
    Or
    
    Select the record and click **Exclude** to exclude the column in the
    generated Excel file and on the
    <span style="font-style: italic;">Data Entry</span> and the
    <span style="font-style: italic;">Mass Change</span> pages.
    
    Or
    
    Select the record and click **Exclude if Null** to exclude the
    column in the generated Excel file if the column contains no data.

6.  Click the **Read Only** check box to enable it if the data from the
    column should display in the generated Excel file and on the
    <span style="font-style: italic;">Data Entry</span> page, but cannot
    be edited.

7.  Click **Vertical View**.

8.  Click **Edit**.
    
    *[View the field descriptions for the Template (Role Excel Column
    Control) page’s Vertical
    View.](../Page_Desc/Template_Role_Excel_Column_Control_H.htm)*

9.  Select an option in the **Column Format** list box.
    
    **NOTE:** The Column Format allows the user to determine the data
    type of the column in the dspCompose™ generated spreadsheet.

10. Select a background color for the column from the **Background
    Color** list box.

11. Select a text color for the column text from the **Text Color** list
    box.

12. Select a data source from the **List Data Source ID** list box if
    the column type is list box.
    
    **NOTE:** The List Data Source ID is the data source that contains
    the view or table used in a list box.

13. Select a list source from the **List Source** list box if the column
    type is list box.
    
    **NOTE:** The List Source is the view or table that contains the
    values used in a list box.

14. Select a list value from the **List Value** list box if the column
    type is list box.
    
    **NOTE:** The List Value is the column that contains the value used
    within a list box.

15. Select a list display from the **List Display** list box if the
    column type is list box.
    
    **NOTE:** The List Display contains the display value used in a list
    box to the user.

16. Click **Save**.
