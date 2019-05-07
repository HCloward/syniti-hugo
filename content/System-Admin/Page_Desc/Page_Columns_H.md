+++
title = 'Page Columns H'
solution = 'Platform'
+++

# Page Columns H

[Page Columns V](#Page_Columns_V)

<div class="use">

Use this page to

  - [Configure Columns for
    Exporting](../Use_Cases/Exclude%20Columns%20Excel%20Integration.htm)
  - [Add a Control Type to a
    Column](../../WebApp_Dev/Add%20a%20Control%20Type%20to%20a%20Column.htm)
  - [Link to a Page Using Buttons and
    Images](../../WebApp_Dev/Link_to_a_Page_Using_Buttons_and_Images.htm)
  - [Add a Toolbar Button](../Use_Cases/Add%20a%20Toolbar%20Button.htm)
  - [Set Column Control
    Status](../../WebApp_Dev/Set_Column_Control_Status.htm)
  - [Set a Column's Format](../../WebApp_Dev/Set_a_Columns%20Format.htm)
  - [Set Default Field Value for a
    Column](../../WebApp_Dev/Set_Default_Field_Value_for_a_Column.htm)
  - [Add an HTML Area to a
    Column](../../WebApp_Dev/Add_an_HTML_Area_to_a_Column.htm)
  - [Enable Dynamic Image](../../WebApp_Dev/Enable_Dynamic_Image.htm)
  - [Add a Label](../../WebApp_Dev/Add_a_Label.htm)
  - [Add a tab](../../WebApp_Dev/Add_a_Tab.htm)
  - [Enable Show in
    Navigation](../../WebApp_Dev/Enable_Show_in_Navigation.htm)
  - [Set Spanning
    Properties](../../WebApp_Dev/Set_Spanning_Properties.htm)
  - [Enable File Upload and
    Download](../../WebApp_Dev/Enable_File_Upload_Download.htm)
  - [Add List Boxes and Combo
    Boxes](../../WebApp_Dev/Add_List_Boxes_and_Combo_Boxes.htm)
  - [Add a Watermark](../../WebApp_Dev/Add_a_Watermark.htm)
  - [Add a Tooltip](../../WebApp_Dev/Add_a_Tooltip.htm)
  - [Enable Electronic
    Signature](../../WebApp_Dev/Enable_Electronic_Signature.htm)
  - [Assign Column
    Properties](../../WebApp_Dev/Assign_Column_Properties.htm)
  - [Link to a Report from a
    Page](../../WebApp_Dev/Link_to_a_Report_from_a_Page.htm)
  - [Include all Page Details in
    Reports](../../WebApp_Dev/Include_All_Page_Details_in_Reports.htm)
  - [Set Required Fields](../../WebApp_Dev/Set_Required_Fields.htm)
  - [Create Chart Drill
    Down](../../WebApp_Dev/Create_Chart_Drill_Down.htm)

</div>

There are three ways to access this page:

  - Select **Admin \> WebApps** in the *Navigation* pane, and click
    **Pages** for a WebApp. Locate the page and click **Column
    Properties**.
  - Navigate to the page in the WebApp where the column property is to
    be applied. Click **Change Settings** on the Site Toolbar, click
    **Design**, then click **Column Properties**.
  - Navigate to the page in the WebApp where the column property is to
    be applied, right-click the column heading, and click **Add** or
    **Edit (Control Name**) if the column property already exists.

 

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>COLUMN</p></td>
<td><p>Displays either:</p>
<ul>
<li>The name of the column from the view or table associated with the page.</li>
<li>The name of the tab or label</li>
<li>The name of the toolbar button</li>
</ul></td>
</tr>
<tr class="odd">
<td><p><span id="Page Column View Type" class="popUpLink">VIEW TYPE</span></p></td>
<td><p>Displays the context in which the control appears as configured.</p>
<p><em>All Views</em> can be used in most cases. However, column properties can be applied to other views as needed. For example, a field can be a Combo Box on the <em>Horizontal</em> View, but can be a display only field on the <em>Vertical</em> View. In this case, set the field as a Combo Box for the View Type of All Views. Add another record for the field and select a View Type of Vertical, and set the CONTROL STATUS to Disabled.</p></td>
</tr>
<tr class="even">
<td><p>CONTROL</p></td>
<td><p>Displays the behavior of columns within a page. By default, all controls are text boxes but can be overridden by assigning a column property. A column can have one control per view. Refer to <a href="../../WebApp_Dev/Add%20a%20Control%20Type%20to%20a%20Column.htm">Add a Control Type to a Column</a> for more information.</p>
<p><strong>NOTE:</strong> The types of controls available for a column depend on that column's page's page type. Refer to <a href="../../WebApp_Dev/View%20the%20Controls%20Available%20For%20A%20Page%20Type.htm">View the Controls Available for a Page Type</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>LIST SOURCE</p></td>
<td><p>Displays the source of the data when the Control Type is Combo Box or List Box. The value can either be a SQL object (Table or View) or a List Data Provider plugin.</p>
<p>Refer to <a href="../../WebApp_Dev/Add_List_Boxes_and_Combo_Boxes.htm">Add List Boxes and Combo Boxes</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>LINK TO PAGE</p></td>
<td><p>Displays the Page Name/ID the platform navigates to when a page link is performed.</p>
<p>This option can be set for control types:</p>
<ul>
<li>Text Box</li>
<li>Date time</li>
<li>Combo Box</li>
<li>Numeric</li>
<li>List Box</li>
<li>Image</li>
<li>Button</li>
<li>Toolbar</li>
<li>Text Area</li>
</ul>
<p>Refer to <a href="../../WebApp_Dev/Link_to_a_Page_Using_Buttons_and_Images.htm">Link to a Page Using Buttons and Images</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>CONTROL STATUS</p></td>
<td><p>Displays whether the column should be enabled (displayed), disabled (display only), or hidden in the associated View Type.</p>
<p>Control Status can be overridden using Page properties, UserControlView, PageControlView or DataControlViews.</p>
<p>Refer to <a href="../../WebApp_Dev/Set_Column_Control_Status.htm">Set a Column Control Status</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Help</p></td>
<td><p>Click to open the <em>Catalog Phrase Translations (Page Specific)</em> page to set up help text for this column for a specific catalog. The translation displays when a user hovers over the column header.</p></td>
</tr>
</tbody>
</table>

## <span id="Page_Columns_V"></span>Page Columns V

**NOTE:** The fields that display on the *Vertical* View of this page
depend on the control type of the selected column.

## Page Columns V: Label Control Type

<div class="use">

Use this page to [Add a Label.](../../WebApp_Dev/Add_a_Label.htm)

</div>

Field

Description

Column

Displays the text that appears on the Label.

<span id="Page Column View Type" class="popUpLink">View Type </span>

Displays the type that uses the control.

Control

Displays Label.

Basic Properties

Collapse

If enabled, a plus or minus sign displays next to the label. The user
can click it to expand or collapse the display of the fields under that
label's section.

## Page Columns V: tab Control Type

<div class="use">

Use this page to [Add a Label.](../../WebApp_Dev/Add_a_Tab.htm)

</div>

Field

Description

Column

Displays the name of the tab.

<span id="Page Column View Type" class="popUpLink">View Type </span>

Displays the type that uses the control.

Control

Displays tab.

Basic Properties

Collapse

If enabled, a plus or minus sign displays next to the label. The user
can click it to expand or collapse the display of the fields under that
label's section.

## Page Columns V: All Other Control Types

This page contains the following tabs:

  - [General](#General)
  - [Excel](#Excel)
  - [Advanced Properties](#Advanced_Properties)
  - [Enable/Disable Control](#Enable/D)
  - [Deprecated Properties](#Deprecated_Properties)
  - [Spanning Properties](#Spanning)
  - [Relational](#Relational)

## <span id="General"></span>General

Field

Description

Column Description

Column

Displays the name of the column from the view or table associated with
the page.

<span id="Page Column View Type" class="popUpLink">View Type</span>

Displays the context in which the control appears as configured.

All Views can be used in most cases. However, column properties can be
applied to other views as needed. For example, a field can be a Combo
Box on the *Horizontal* View, but can be a display only field on the
*Vertical* View. In this case, set the field as a Combo Box for the View
Type of All Views. Add another record for the field and select a View
Type of Vertical, and set the CONTROL STATUS to Disabled.

Control Status

Displays whether the column should be enabled (displayed), disabled
(display only), or hidden in the associated View Type.

Refer to [Set a Column Control
Status](../../WebApp_Dev/Set_Column_Control_Status.htm) for more
information.

Control

Displays the behavior of columns within a page. By default, all controls
are text boxes but can be overridden by assigning a column property. A
column can have one control per view. Refer to [Assign a Control Type to
a
Column](../../WebApp_Dev/Add%20a%20Control%20Type%20to%20a%20Column.htm)
for more information.

Basic Properties

Image ID

Displays the name of the image used for the button or image.

This field displays for the controls:

  - Image
  - Button
  - Toolbar

Link to Page ID

Displays the name of the page that opens when the user clicks the
control.

Refer to [Link to a Page using Buttons and
Images](../../WebApp_Dev/Link_to_a_Page_Using_Buttons_and_Images.htm)
for more information.

This field displays for the controls:

  - Image
  - Button
  - Text Area
  - Toolbar

Required

Displays the requirement level on a column by adding a page validation
view. The requirement levels are:

  - **Required (Hard)** – This setting specifies this field must contain
    valid data before a save can be completed.
  - **Required (Soft)** - This setting generates an error but allows
    records to be saved.
  - **No** – The field is not required.

If the field value contains NOT NULL in the table (such as a key),
columns automatically defaults to Required (Hard).

Refer to [Set Required Fields](../../WebApp_Dev/Set_Required_Fields.htm)
for more information.

This field displays for the controls:

  - Combo Box
  - HTML Area
  - Text Box
  - DateTime
  - Numeric
  - List Box
  - Text Area

Default

Provides defaults for page columns during record insert. Defaults may
also be set by a Defaults View at the page level.

Refer to [Set the Default Field Value for a
Column](../../WebApp_Dev/Set_Default_Field_Value_for_a_Column.htm) for
more information.

This option is available for these controls:

  - Check Box
  - Combo Box
  - HTML Area
  - Text Box
  - DateTime
  - Numeric
  - List Box
  - Text Area

Checkbox Format ID

Displays the format. Options are:

  - SAP BDC

**NOTE:** A check box using this format allows the values ‘X’ for
checked and ‘\!’ for unchecked. The ‘\!’ is a special character used in
an SAP BDC that tells the program there is no data in the field (i.e.,
the field should be ignored). This is useful when doing an update to
existing data in SAP and the data must not change unless it has been
modified.

  - SAP Checkbox – Deprecated

**NOTE:** A check box using this format allows the values ‘X’ for
checked and ‘ ‘ for unchecked.

  - Y or N

**NOTE:** A check box using this format allows the values ‘Y’ for
checked and ‘N’ for unchecked.

**NOTE:** If the data type of the table column in SQL is set to bit, the
DSP® assumes the field is a checkbox and appropriately populate the data
with a 1 or 0.

**NOTE:** If one of these formats is chosen for the checkbox, the data
type of the table column in SQL must be set to a character of length 1.
The user will receive a hard error while entering data on the page if
one of these checkbox formats is selected and the data type of the field
is bit or another non-character format.

**NOTE**: This option is available for Check Box only.

Watermark Text

Displays static text to use as a placeholder watermark when the control
is empty.

Refer to [Add a Watermark](../../WebApp_Dev/Add_a_Watermark.htm) for
more information.

This field displays for the controls:

  - Combo Box
  - HTML Area
  - Text Box
  - DateTime
  - Numeric
  - List Box
  - Text Area

Format

Displays a format for the selected control specified by the page
Designer. Options vary for each control. Column database type should be
taken into consideration when selecting Numeric and DateTime formats.

Refer to [Set a Column’s
Format](../../WebApp_Dev/Set_a_Columns%20Format.htm) for more
information.

This field displays for the controls:

  - Text Box
  - DateTime
  - Numeric
  - Text Area

Move To Toolbar

Displays the toolbar location. The only option is Page.

This field displays for the Toolbar control only.

Basic List Properties

**NOTE:** The fields in this section display for List Box and Combo Box
controls only.

List Source

Displays the source of the data when the Control Type is Combo Box or
List Box. The value can either be a SQL object (Table or View) or a List
Data Provider plugin.

Refer to [Add List Boxes and Combo
Boxes](../../WebApp_Dev/Add_List_Boxes_and_Combo_Boxes.htm) for more
information.

List Value Field

Displays the name of the field that stores the value.

In most cases, List Value Field is the primary key stored in the table

Refer to [Add List Boxes and Combo
Boxes](../../WebApp_Dev/Add_List_Boxes_and_Combo_Boxes.htm) for more
information.

List Display Field

Displays the option visible in the List Box or Combo Box.

Refer to [Add List Boxes and Combo
Boxes](../../WebApp_Dev/Add_List_Boxes_and_Combo_Boxes.htm) for more
information.

Basic List Properties

**NOTE:** The fields in this section display for the File control only.
Refer to [Enable File
Upload/Download](../../WebApp_Dev/Enable_File_Upload_Download.htm) for
more information.

File Path

Displays the path name to upload files to and to store files for
download

**NOTE:** The files are usually stored in a folder with the same name as
the DSP® WebApp ID (GUID). Use the forward slash / within and at the end
of the path. The forward slash at the end of the path denotes a folder.
For example, if /NWEmployees is used, it is treated as a file name.
/NWEmployees/employee/ is treated as a folder.

**NOTE:** The folder UserArea is created by DSP® and should always be
the first folder name in the path. The English folder is required and
must be added by the user. The WebApp ID sets the path to the WebApp.
Other folders or sub folders can be used but the English folder is used
as the default.

File Path Type

Displays the path type. Options are:

  - **Data Source** – Stores the file in the directory configured for an
    existing Local File type Data Source. The File Data Source Field
    must be populated when this option is selected
  - **Virtual** – Stores the file internally in the WebApp.
  - **Physical** – Stores the file in a separate location from the
    internal web app directories.

File Direction

Displays whether the file can be uploaded only, downloaded only, or both
uploaded and downloaded.

File Data Source Field

Displays the data source with a Data Source Type of Local File, and used
with File Path Type set to Data Source. Path is a required field on a
Local Path type Data Source and contains the location where these
uploaded files will be placed.

**NOTE:** The fields in this section display for the Numeric control
only.

Numeric Scale

Displays the number of decimal places to display after the decimal
separator.

Display Thousands Separator

If enabled, a number uses the current user’s locale to display a number
such as 4213.22 as 4,213.22 given that English – United States is
selected in the Currency Locale ID List Box.

Currency Locale ID

Displays the locale used for formatting currency.

Total

If enabled, a totals column recalculates when records are added,
deleted, or modified.

<span id="Advanced_Properties"></span>

### Advanced Properties

Field

Description

Header Image ID

Displays the image to appear in the header row for this column.

This field displays for these controls:

  - HTML Area
  - Text Box
  - Button
  - Check Box
  - DateTime
  - Combo Box
  - Image
  - File
  - Numeric
  - List Box
  - Text Area

Header Image

Displays a depiction of header image chosen.

This field displays for these controls:

  - HTML Area
  - Text Box
  - Button
  - Check Box
  - DateTime
  - Combo Box
  - Image
  - File
  - Numeric
  - List Box
  - Text Area

Dynamic Image

If enabled, the Image specified displays in the contents of the query.
Using the power of the conditional "IF" statement in the query, the
image may vary according to value of data for each row.

If not enabled, the image specified does not display.

This field displays for these controls:

  - Text Box
  - Date time
  - Image
  - Numeric

Hover View

Displays the name of the view created in SQL that populates the hover
view for the column.

This value can be set at the page level as well. The Hover View can be
populated with additional technical information about the selected
record.

This field displays for these controls:

  - Combo Box
  - List Box

Dynamic Link Type

Displays the dynamic link method the control uses when the image is
clicked. Options are:

  - **Dynamic Pages** – This option contains a platform PageID.
  - **Dynamic Views** – this option is comprised of SQL statements that
    can use drill or binding criteria...
  - **Dynamic URLs** – This option must contain a URL.

This field displays for these controls:

  - Text Box
  - Button
  - Date time
  - Image
  - Numeric
  - Toolbar

Dynamic Link Column

Displays the column in view to use as dynamic link criteria.

Dynamic Links may be used to navigate to WebApp pages outside of the
current WebApp.

This field displays for these controls:

  - Text Box
  - Button
  - Image

Link To Page ID

Displays the platform page name navigated to when page link is executed.
Value list only contains pages in the current WebApp. Dynamic Links may
be used to navigate to WebApp pages outside of the current WebApp.

This field displays for these controls:

  - Text Box
  - Date time
  - Combo Box
  - Numeric
  - List Box
  - Image
  - Toolbar
  - Text Area

Link to Method

Displays whether the page that is accessed from the control overlays the
existing page or opens in a separate page.

This field displays for these controls:

  - Button
  - Image
  - List
  - Toolbar

Runtime Data Source ID

Displays the field name that contains a GUID that corresponds to the
Data Source to join against for the view/table specified in the List
Table column.

The DSP® looks for that field's value in the following order.

1.  Column in the page's horizontal or vertical view
2.  Drill Down Criteria passed to this page.
3.  Link Criteria passed to this page.
4.  Shared Criteria for this WebApp.

The System Administration WebApp uses this feature extensively to look
up INFORMATION\_SCHEMA objects. For example, when looking up column
names, the DSP® creates a boaColumnList view in the database when a data
source is registered, as opposed to relying on one view that unions the
INFORMATION\_SCHEMA views of all data sources. Connecting to the actual
Data Source directly increases performance, reliability and scalability.

This field displays for these controls:

  - Button
  - Combo Box
  - Image
  - List Box
  - Toolbar

Key

If enabled, the selected column name is a primary key. The platform only
passes Primary Keys when linking to other pages. If the page data source
is a view, a control must be added indicating the Key.

If disabled, the selected column name is not a primary key.

This field displays for these controls:

  - Check Box
  - Text Box
  - Date time
  - Combo Box
  - List Box
  - File
  - Numeric
  - Text Area

Allow Space

If enabled, a required column is allowed to have space(s) as a valid
entry. If disabled, a required column is not allowed to have space(s) as
a valid entry.

This field displays for these controls:

  - Text Box
  - Date time
  - Combo Box
  - Numeric
  - List
  - Text Area

Require Signature

If enabled, a panel appears requiring the current session UserID and
Password to save changes. Applies to both record Insert and Update. The
panel will not appear if logged in as an Anonymous user. Requires
auditing to be enabled for the underlying page table and column.

If not enabled, changes are automatically saved without the UserID and
Password of the current user.

Refer to [Enable Audit Trail and Electronic
Signature](../../WebApp_Dev/Enable_Audit_Trail_Electronic_Signature.htm)
for more information.

This field displays for these controls:

  - HTML Area
  - Text Box
  - Check Box
  - Date time
  - Combo Box
  - File
  - Numeric
  - List Box
  - Text Area

Wrap

If enabled, the text associated with the label for the check box wraps.

This field displays for the Check Box control only.

Show In Navigation

If enabled, the column displays in the Navigation pane as a value when
the page title is expanded in the Navigation pane. By default it
displays the Primary Key from the underlying table.

Refer to [Enable Show in
Navigation](../../WebApp_Dev/Enable_Show_in_Navigation.htm) for more
information.

This field displays for these controls:

  - Text Box
  - List Box

Translate

If enabled, the cell values are translated. Translations are dependent
on catalog entries for the selected session Language. Refer to [Manage
Catalogs](../Use_Cases/Manage_Catalogs.htm) for more information.

If disabled, the cell values are not translated.

This field displays for these controls:

  - Text Box
  - Combo Box
  - Image
  - List Box
  - Toolbar
  - Text Area

**NOTE:** The fields in this section display for the Text Area control
type only.

Binding Field Names

Displays a comma-separated list of columns used to filter data on a
linked page. By default, when linking form one page to another, the DSP®
sends the key fields to the linked page. However, it the key fields are
different between linked pages or additional fields are required, use
this field to indicate the columns.

For instance, a user clicks a button on a page listing country records
to access a page listing the selected country’s regions. If both pages
do not have the country field with the same name, the field on the
linked page must be added here to include as part of the binding
criteria. Otherwise, the region page displays regions for all countries.

Shared Field Names

Displays a comma-separated list of columns used to send data to a linked
page.

Shared Fields tell the DSP® to send the data from a column that is not
normally passed and allow it to be used on a subsequent page. For
example, to filter a Region list box on a page by the Country field that
was entered on a previous page, add the Country field as a shared field
on the link between pages. It is then available for use in the list box
Where Clause on the Region page.

If you were to include Country as a Shared Field and not a Binding
Field, you would see regions for all countries after clicking the link,
but any list boxes with a Country filter would only show regions
filtered by the country shared from the previous page.

**NOTE:** The fields in this section display for the Toolbar control
type only.

Consider Valid

If enabled, the boaStatus column is used to determine whether the
toolbar button is active or dimmed.

Refer to [Use boaStatus to Set a Toolbar Button’s Control
Status](../../WebApp_Dev/Use%20boaStatus%20to%20Set%20a%20Toolbar%20Buttons%20Control%20Status.htm)
for more information.

Allow Multi Row Action

If enabled, a user can select multiple records on the Horizontal View
and click the toolbar button to perform the action related to the
toolbar button on multiple records at once.

**NOTE:** The fields in this section display for the Image control type
only.

Report Follows Link

If enabled, generates a report for the current Dynamic page for the
*Horizontal* or *Vertical* Views.

Refer to [Include all Page Details in
Reports](../../WebApp_Dev/Include_All_Page_Details_in_Reports.htm) for
more information.

Link to Report

If enabled, when a user clicks the image, the page to access opens in a
read-only format.

By default, page links render data using the normal *Horizontal* or
*Vertical* View with add/edit/delete capability. Link to Report provides
a mechanism to report data as read-only without having to modify
defaulted page properties.

Refer to [Link to a Report from a
Page](../../WebApp_Dev/Link_to_a_Report_from_a_Page.htm) for more
information.

Advanced List Properties

**NOTE:** The fields in this section display for List Box and Combo Box
controls only.

List Where Clause

Displays the Where Clause used to restrict the values that display in a
List Box or Combo Box.

Refer to [Set a Dynamic List
Box](../../WebApp_Dev/Set_a_Dynamic_List_Box.htm) and [Enable List Where
Clause](../../WebApp_Dev/Enable_List_Where_Clause.htm) for more
information.

List Order By

Displays the column that sets the sort for values in the List Box or
Combo Box.

By default, like pages, List Boxes are sorted based on the primary key.
Use List Order By to sort select options in a List Box based on another
field.

**NOTE:** When a field name is entered in List Order By field, the
default order is ascending. To sort in descending order, enter the field
name followed by a space and desc, for example, ProductName desc.
Separate entries by a comma.

List Unique

if enabled, displays List Box or Combo Box values not previously
selected in another record on the page. If the record has already been
added, the List Unique property removes it from the List Box, leaving
only the records that have not been selected.

List Filter

If enabled, the Filter icon displays next to the Combo Box, indicating a
filter is enabled.

The Combo Box Filters are designed to reduce the number of items
displayed in the value field or the descriptive field.

**NOTE:** This field displays for the Combo Box control only.

List Allow Insert

Displays an option that sets the behavior of the List Box or Combo Box
when the value stored in the field is known.

As the user types in the List Box, matching values display.

Options for List Allow Insert are:

  - **No** – Insert does not display and additional options cannot be
    added or searched.
  - **Yes** – Insert displays and any additional option can be entered
    in the field regardless of the options available in the List Box.
    The record is considered valid. The added value does not become a
    future option in the table.
  - **Constrained to List Source** –A user can add a new entry by
    clicking Use this Value. A validation rule automatically runs to
    verify the entry is valid. This prevents undesirable data being
    added to the list table.

**NOTE:** The current user must have security to add new records to the
page associated with the list.

List Allow Insert Page ID

Displays the name of the page that displays when a user clicks a link
that displays below the List Box that allows them to add a new record.
Used in conjunction with List Allow Insert. This feature permits
additional values not available in the list to be added to the
associated list.

If both are enabled, clicking the link opens a window containing the
page associated with the list. Enter the new options in the fields and
the value is available in the List Box when adding new records.

List Selection Field

Displays the name of the field that contains descriptive text that
displays in a List Box or a Combo Box when in add or edit mode. Refer to
[Add a List Selection
Field](../../WebApp_Dev/Add_a_List_Selection_Field.htm) for more
information.

List Control View

Displays the name of the view used to select columns from the table to
restrict the number of values in the List Box or Combo Box.

## <span id="Excel"></span>Excel

**NOTE:** This tab displays if Excel Integration is enabled. Refer to
[Enable Excel Integration](../Use_Cases/Enable_Excel_Integration.htm)
for more information

It displays for these control types:

  - Text Box
  - Check Box
  - Text Area
  - List Box,
  - Numeric
  - Combo Box
  - DateTime
  - HTML
Area

|                        |                                                                     |
| ---------------------- | ------------------------------------------------------------------- |
| Field                  | Description                                                         |
| Excel Foreground Color | Displays the foreground color to use on Excel template header rows. |
| Excel Background Color | Displays the background color to use on Excel template header rows. |

## <span id="Deprecated_Properties"></span>Deprecated Properties

**NOTE:** This tab does not display for the Toolbar control.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Wrap</p></td>
<td><p>If enabled, the text associated with the label for the check box wraps.</p>
<p>This field displays for the control types:</p>
<ul>
<li>Button</li>
<li>Combo Box</li>
<li>DateTime</li>
<li>File</li>
<li>List Box</li>
<li>Numeric</li>
<li>Text Area</li>
<li>Text Box</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Control Function</p></td>
<td><p>This field is not used.</p></td>
</tr>
</tbody>
</table>

## <span id="Enable/D"></span>Enable/Disable Control

<div class="use">

Use this tab to [Set Column Control
Status](../../WebApp_Dev/Set_Column_Control_Status.htm).

</div>

**NOTE:** This tab does not display for the Toolbar control.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Consider Valid</p></td>
<td><p>If checked, the boaStatus column is used to determine whether the control is enabled or disabled.</p>
<p>If unchecked, and the Control Status Field on the Enable/Disable tab displays another column in the view, this column’s value (NULL/0, 1, or 2) determines the Control Status of this column for a given row.</p>
<p>If unchecked and the Control Status Field is blank, the control status field is not set using either of these methods. Control Status can also be set as a column property. Refer to <a href="../../WebApp_Dev/Set_Column_Control_Status.htm">Set Column Control Status</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Control Status Field</p></td>
<td><p>Displays the name of the column in the view whose value (NULL/0, 1, or 2) determines the Control Status of this column for a given row. Refer to <a href="../../WebApp_Dev/Set_Column_Control_Status.htm">Set Column Control Status</a> for more information.</p></td>
</tr>
</tbody>
</table>

## <span id="Spanning"></span>Spanning Properties

<div class="use">

Use this tab to [Set Spanning
Properties](../../WebApp_Dev/Set_Spanning_Properties.htm).

</div>

|             |                                                                                                                                                                                              |
| ----------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field       | Description                                                                                                                                                                                  |
| Column Span | Displays the number of display columns that this column extends through. For example, if the Column Span is 2, the selected column displays its contents over two columns instead of one.    |
| Row Span    | Displays the number of display rows that this column extends through.                                                                                                                        |
| Line Break  | If enabled, a new display row is created after the selected column. If disabled, a new display row is not created after the selected column and subsequent controls stay on the current row. |

## <span id="Relational"></span>Relational

**NOTE:** This tab does not display for a Check Box, File, or Toolbar
control.

<div class="use">

Use this tab to:

  - [Add a Watermark](../../WebApp_Dev/Add_a_Watermark.htm)
  - [Add a Tooltip](../../WebApp_Dev/Add_a_Tooltip.htm)

</div>

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Watermark View</p></td>
<td><p>Displays the view that defines what text should appear for each record when the field is empty as an informational watermark.</p>
<p>This field displays for the controls:</p>
<ul>
<li>HTML Area</li>
<li>Text Box</li>
<li>Date Time</li>
<li>Combo Box</li>
<li>Numeric</li>
<li>List Box</li>
<li>Text Area</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Watermark Binding Field Names</p></td>
<td><p>Displays the fields to bind page data against watermark view with.</p>
<p>This field displays for the controls:</p>
<ul>
<li>HTML Area</li>
<li>Text Box</li>
<li>Date Time</li>
<li>Combo Box</li>
<li>Numeric</li>
<li>List Box</li>
<li>Text Area</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Translate Watermark</p></td>
<td><p>If enabled, the watermark value is run through system translation. If disabled, the watermark value is not translated.</p>
<p>This field displays for the controls:</p>
<ul>
<li>Text Box</li>
<li>HTML Area</li>
<li>Date Time</li>
<li>Combo Box</li>
<li>Numeric</li>
<li>List Box</li>
<li>Text Area</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Data Tooltip View</p></td>
<td><p>Displays the name of the view that contains the tooltip. Before creating a tooltip, the user mist write a view with the suffix Dtv for each column that requires a tooltip and alias the column as boatooltip? in the view.  </p>
<p>This field displays for the controls:</p>
<ul>
<li>Button</li>
<li>Combo Box</li>
<li>Image</li>
<li>List Box</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Data Tooltip Binding Field Names</p></td>
<td><p>Displays the comma-delimited list of field names to bind against to return tooltip data.</p>
<p>For instance, if you wanted the page to display a different tooltip depending on data from a previously populated field, you could use that field here as a binding column allowing it to select the proper data to display.</p>
<p>This field displays for the controls:</p>
<ul>
<li>Button</li>
<li>Combo Box</li>
<li>Image</li>
<li>List Box</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Translate Tooltip</p></td>
<td><p>If enabled, the tooltip value is run through system translation. If disabled, the watermark value is not translated.</p>
<p>This field displays for the controls:</p>
<ul>
<li>Button</li>
<li>Combo Box</li>
<li>Image</li>
<li>List Box</li>
</ul></td>
</tr>
</tbody>
</table>
