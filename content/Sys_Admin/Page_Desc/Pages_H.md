+++
title = 'Pages H'
solution = 'Platform'
+++

# Pages H

[Pages V](#Pages_V)

<div class="use">

Use this page to:

  - [Configure Business Rule
    Settings](../Use_Cases/Configure_Business_Rule_Settings)
  - [Create a Chart Page](../../WebApp_Dev/Create_a_Chart)
  - [Design Pages](../../WebApp_Dev/Page%20Design%20Guidelines)
  - [Create a Dynamic
    Page](../../WebApp_Dev/Register_a_Dynamic_Page)
  - [Assign Page Properties to a Dynamic
    Page](../../WebApp_Dev/Assign_Page_Properties)
  - [Create a Header Detail
    Page](../../WebApp_Dev/Create_Header_Detail_Pages)
  - [Create a Static
    Page](../../WebApp_Dev/Create%20a%20Static%20Page)
  - [Create a Service
    Page](../../WebApp_Dev/Create%20a%20Service%20Page)
  - [Create a Chart Page](../../WebApp_Dev/Create_a_Chart)
  - [Create a Dashboard Page](../../WebApp_Dev/Create_a_Dashboard)
  - [Create a Report Page](../../WebApp_Dev/Create%20Report%20Pages)
  - [Copy a Page in a
    WebApp](../../WebApp_Dev/Copy_a_Page_in_a_WebApp)

</div>

To access this page:

1.  Select **Admin \> WebApps** in the *Navigation* pane.

2.  Click the **Pages** icon for a **WEB APP NAME**.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays the name of the page used to identify the page in menus and lists. Any alpha-numeric string may be used.</p></td>
</tr>
<tr class="odd">
<td><p>PAGE TYPE</p></td>
<td><p>Displays the page type of the selected record.</p>
<ul>
<li><strong>Chart</strong> — Pages of this type display data in a visual format for easier interpretation. Some types include Line, Bar, and Pie.</li>
<li><strong>Dashboard</strong> — Pages of this type contain Layouts which allow the Designer to render several Chart pages at once depending on the configured layout.</li>
<li><strong>Dynamic</strong> — Pages of this type are the standard pages of the framework that allow for configured column controls and data manipulation.</li>
<li><strong>Header Detail</strong> — Pages of this type display two linked pages in parent and dependent panes.</li>
<li><strong>Report</strong> — Pages of this type are used as read-only renderings of data similar to Dynamic pages. With this page type, an automatic “Reports” link is added to the applications switchboard and each report page is shown as a page link.</li>
<li><strong>Service</strong> — Pages of this type are configured to run events on a pre-defined interval. Both unit of measurement and quantity of measurement can be defined. These run in the background.</li>
<li><strong>Static</strong> — Pages of this type allow the Designer to embed an external resource, whether a file, .aspx page, or other web resources.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>TABLE</p></td>
<td><p>Displays the name of the table or view where changes will be stored.</p>
<p>A table must be defined on all Dynamic pages.</p>
<p>A view can be used to update a table in another database. When using this advanced method, the key field(s) for the foreign table must be defined in Column properties.</p>
<p>Refer to <a href="../../WebApp_Dev/Assign_Column_Properties">Assign Column Properties</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Column Properties</p></td>
<td><p>Click to display the <em><a href="Page_Columns_H">Page Columns</a></em> page where Control Properties are used to control the behavior of columns within a page. By default, all controls are text boxes, but you can override this behavior using column properties. All standard browser controls are available.</p>
<p>Refer to <a href="../../WebApp_Dev/Assign_Column_Properties">Assign Column Properties</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Events</p></td>
<td><p>Click to open the <em><a href="Page_Events_H">Page Events</a></em> page to add and view business rules, workflow views and validation rules for the page.</p></td>
</tr>
<tr class="odd">
<td><p>Page Groups</p></td>
<td><p>Click to open the <em><a href="Page%20Groups">Page Groups</a></em> page to set page security for WebApp groups. This includes which Groups can view, edit, delete, and insert records.</p></td>
</tr>
<tr class="even">
<td><p>Security Definitions</p></td>
<td><p>Click to open the <em><a href="Security_Definition_Pages">Security Definition Pages</a></em> page to add and view the security definitions integrated into this page. These definitions are bound on page columns and are used to restrict the availability of data through Role Security. Refer to <a href="../Use_Cases/RegSecurityDefCompsWebApps">Register Security Definitions to Components (WebApps)</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Edit Page Help</p></td>
<td><p>Click to open the <em>Catalog Page Help</em> page, where the user can set the Dynamic Subtitle which appears when the page is loaded. These are defined per language.</p></td>
</tr>
</tbody>
</table>

## <span id="Pages_V"></span>Pages V

[Pages H](#Pages_H)

**NOTE:** The page type determines the fields that display on the Pages
*Vertical* View.

  - [Dynamic](#Dynamic)
  - [Static](#Static)
  - [Header Detail](#Header)
  - [Chart](#Chart)
  - [Dashboard](#Dashboar)
  - [Service](#Service)
  - [Report](#Report)

## <span id="Dynamic"></span>Dynamic Page Type V (All tabs)

This page contains the following tabs:

  - [General tab](#DynamicPageGeneraltab)
  - [Control Views tab](#DynamicControlViewstab)
  - [Advanced Properties tab](#DynamicAdvPropstab)
  - [Excel tab](#DynamicExceltab)
  - [Report Options tab](#DynamicReportOptionstab)
  - [Search Options tab](#DynamicSearchOptionstab)
  - [Deprecated Properties tab](#DynamicDepPropstab)

<div class="use">

Use this page to [Create a Dynamic
Page.](../../WebApp_Dev/Register_a_Dynamic_Page)

</div>

## <span id="DynamicPageGeneraltab"></span>Dynamic Page Type: General tab

Field

Description

Description

Displays the page name.

Page Type

Displays the page type, in this case Dynamic.

Basic Properties

Table

Displays the name of the table where the data for the page is stored.

Horizontal View

Displays the SQL View that determines what fields from the table are to
display on the *Horizontal* View of the page, in what order.

Order By

Displays the name of the column on the *Horizontal* View that is the
default sort on the page. The column sorts in either ascending or
descending order. Sorting must be done in the DSP®, not in the SQL view.

**NOTE:** When a field name is entered in Order By field, the default
order is ascending. To sort in descending order, enter the field name
followed by a space and desc, for example, lastname desc. Separate
entries by a comma. If the page is sorted by multiple columns, a number
displays next to each column header indicating the order of the sort.

Vertical View

Displays the SQL View that determines what fields from the table are to
display on the *Vertical* View of the page, in what order.

Horizontal Menu ID

Displays the menu that displays to the left of the page when the page is
accessed. The standard menu is {component name} : Switchboard.

Vertical Menu ID

This field is not used.

Insert Method

Displays the page behavior when adding a new record. Options are:

  - **Not Supported** — No records can be added to the page. The Add
    icon on the Page toolbar does not display.
  - **Horizontal Insert** — Once a record is added and saved the current
    *Horizontal* View persists.
  - **Horizontal Insert/Switch to Vertical** — Once the record is added
    and saved, the *Vertical* View displays. The *Vertical* View must be
    saved to save any information on the *Vertical* View only. If the
    *Vertical* View is not saved, the data entered on the *Horizontal*
    View persists and still displays.
  - **Horizontal/Switch to Vertical** — Once the record is added and
    saved, the *Vertical* View displays. The *Vertical* View must be
    saved to save any information on the *Horizontal* and *Vertical*
    Views. If the *Vertical* View is not saved, the data entered on the
    *Horizontal* View is not saved.
  - **Switch to Vertical Immediately** — Upon adding a record, the
    *Vertical* View displays.

Update Method

Displays the page behavior when editing a record. Options are:

  - **Not Supported** — No records can be edited. The Edit icon on the
    Page Toolbar does not display.
  - **Horizontal Update** — Once a record is edited and saved the
    current *Horizontal* View persists.
  - **Horizontal Update/Switch to Vertical** — Once the record is edited
    and saved, the *Vertical* View displays. The *Vertical* View must be
    saved to save any information on the *Vertical* View only. If the
    *Vertical* View is not saved, the data edited on the *Horizontal*
    View persists and still displays.
  - **Horizontal/Switch to Vertical** — Once the record is edited and
    saved, the *Vertical* View displays. The *Vertical* View must be
    saved to save any information on the *Horizontal* and *Vertical*
    Views. If the *Vertical* view is not saved, the data edited on the
    *Horizontal* View is not saved.
  - **Switch to Vertical Immediately** — Upon editing a record, the
    *Vertical* View displays.

Support Delete

If checked, records on the page can be deleted. If unchecked, the Delete
icon does not display on the
page.

## <span id="DynamicControlViewstab"></span>Dynamic Page Type: Control Views tab

Field

Description

Status Control Views

User Control View

Displays the user control view applied to this page.

See [User Control Views](../../WebApp_Dev/User_Control_Views) for
more information.

Page Control View

Displays the page control view applied to this page.

See [Page Control Views](../../WebApp_Dev/Page_Control_View) for
more information.

Data Control View

Displays the data control view applied to this page.

See [Data Control Views](../../WebApp_Dev/Data_Control_Views) for
more information.

Page Views

Toolbar View

Displays the toolbar view applied to this page.

Toolbar views default naming convention: web\*Tbv

Toolbar views are used to create custom buttons at the page toolbar
level. The controls included do not apply to rows and the toolbar
control type is the only control type that can be applied to a column in
a Toolbar view.

Refer to [Add a Toolbar
Button](../Use_Cases/Add%20a%20Toolbar%20Button) for more
information.

Parameter View

Displays the parameter view applied to this page.

Parameter views default naming convention: web\*PV

The results from the parameter view are stored with the other
environmental variables (as in, boaUserID). These variables are used in
places like substituting \#\# variables in list Where clauses and
passing arguments to events.

Hover View

Displays the name of the view created in SQL that populates the hover
view for the page.

Hover views default naming convention: web\*Hov

The Hover View can be populated with additional technical information
about the selected page.

When a record is selected on the page, if the user hovers the cursor
over the page title, after a brief delay, the record’s keys display by
default in the Information pane (below the Navigation pane). These
values are usually GUIDs, which are meaningless to the end user. The
Hover View can be populated with additional technical information about
the selected record.

Column Views

Defaults View

Displays the view name that stores default values for the
page.

## <span id="DynamicAdvPropstab"></span>Dynamic Page Type: Advanced Properties tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Short Description</p></td>
<td><p>Displays a short description of the page for documentation purposes.</p></td>
</tr>
<tr class="odd">
<td><p>Support Persistent Insert</p></td>
<td><p>If checked, when a user adds a record on the page and clicks Save, the page remains in Add mode. This feature is useful when a user adds several records, one after the other.</p></td>
</tr>
<tr class="even">
<td><p>Support Direct Update</p></td>
<td><p>If checked, a user can enable or disable a check box on this page without having to edit the page (as in., click the Edit button). This feature is useful when there is a check box(es) on the page, and updating the check box(es) is commonly the only change that a user makes on the page. Uncheck this setting if it is expected that the user will update additional information on the page besides the check box(es).</p></td>
</tr>
<tr class="odd">
<td><p>Enable Excel Integration</p></td>
<td><p>If checked, Excel integration is available on the page.</p>
<p>Excel Integration is the ability, at the framework level, to enable end-users to import data from Excel into DSP® pages.  </p>
<p>Refer to <a href="../Use_Cases/Enable_Excel_Integration">Enable Excel Integration</a> and <a href="../../Excel_Int/Use_Excel_Integration">Use Excel Integration</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Maintain Page Location</p></td>
<td><p>If checked, when the user adds or edits a record and the page switches to <em>Vertical</em> View, it remains in <em>Vertical</em> View after the user saves the record.</p>
<p>If unchecked, the page returns to the <em>Horizontal</em> View when a record is saved, which is the standard behavior.</p></td>
</tr>
<tr class="odd">
<td><p>Support Download</p></td>
<td><p>If checked, the page allows a user to download data to an Excel spreadsheet, a Word document or other formats.</p>
<p>Use this feature depending on the type of data the page displays, for example, a metric-related page may be useful to download, while a page containing sensitive information may not.</p>
<p><strong>NOTE:</strong> Exclude fields, such as images and buttons, in the downloaded file if needed. Refer to <a href="../../WebApp_Dev/Set_Column_Control_Status">Set Column Control Status</a> for more information.</p>
<p><strong>NOTE:</strong> In a case where fields should be included on the Download page that are not visible on the <em>Horizontal</em> or <em>Vertical</em> View, hide fields using the page columns All Views view type, but then enable them on the Download for this level of control.  Refer to <a href="../../WebApp_Dev/Enable_File_Upload_Download">Enable File Upload/Download</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Refresh Rate</p></td>
<td><p>Displays the amount of time in seconds that passes before the page is automatically refreshed. If the value is 0, the page is not automatically refreshed.</p></td>
</tr>
<tr class="odd">
<td><p>Static Source </p></td>
<td><p>This field is not used.</p></td>
</tr>
<tr class="even">
<td><p>Catalog ID</p></td>
<td><p>Displays the name of the catalog used for translations for this page, if needed.</p>
<p>Refer to <a href="../Use_Cases/Manage_Catalogs">Manage Catalogs</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Allow Explicit Quick Link</p></td>
<td><p>If checked, this page can be linked to using the Quick Links feature. Refer to <a href="../Use_Cases/Quick_Links">Quick Links</a> for more information.</p>
<p>If this page requires binding to function correctly (Page Control View for example), then this setting must be disabled.</p></td>
</tr>
<tr class="even">
<td><p>Copy</p></td>
<td><p>Click to open the <em><a href="Copy%20Page">Copy Page</a></em> page to create a copy of the selected page to use as a basis for a new page. When a page is copied, the column properties, events, validations and other settings are copied.</p>
<p><strong>NOTE:</strong> This button is disabled if the page is in Edit mode. Refer to <a href="../../WebApp_Dev/Copy_a_Page_in_a_WebApp">Copy a Page in a WebApp</a> for more information.</p></td>
</tr>
</tbody>
</table>

## <span id="DynamicExceltab"></span>Dynamic Page Type: Excel tab

**NOTE:** This tab only displays if Excel Integration has been enabled.
See [Enable Excel
Integration](../Use_Cases/Enable_Excel_Integration) for more
information.

Field

Description

Excel Instructions

Displays text that is included in downloaded Excel templates as an
additional 'Instructions' sheet.

Technical Column Name Row

Excel Column Name Background

Displays the background color for the header row containing the
original, untranslated column name.

Excel Column Name Foreground

Displays the foreground color for the header row containing the
original, untranslated column name.

Translated Column Name Row

Excel Translated Name Background

Displays the background color for the header row containing the
translated column name.

Excel Column Name Foreground

Displays the foreground color for the header row containing the
translated column name.

Data Type Row

Excel Data Type Header

If checked, a header row is included in downloaded Excel templates that
displays data type and length details for each column.

Excel Data Type Foreground

Displays the foreground color for the header row containing column data
type details.

Help Text

Excel Help Text as Comment

When checked, in the downloaded Excel template, the column help text is
displayed in comments when hovering over the second row.

See [Add Column Help Text](../../WebApp_Dev/Add_Column_Help_Text)
for more information

Excel Help Text Header

When checked, a header row is included in downloaded Excel templates
that contains a text-only representation of the column's help text
(without HTML markup).

Excel Help Text Background

Displays the background color for the header row containing column help
text.

Excel Help Text Foreground

Displays the foreground color for the header row containing column help
text.

## <span id="DynamicReportOptionstab"></span>Dynamic Page Type: Report Options tab

|                |                                                                                                                                                                                                                    |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field          | Description                                                                                                                                                                                                        |
| Support Report | If checked, the Report option is available on the Page Options drop-down for the page.                                                                                                                             |
| Report View    | Displays the report view used for the report.                                                                                                                                                                      |
| Report Groups  | Click to open the *[Report Groups](Report%20Groups)* page to create report groups to organize the report. Refer to [Create Report Groups](../../WebApp_Dev/Create%20Report%20Groups) for more information. |

## <span id="DynamicSearchOptionstab"></span>Dynamic Page Type: Search Options tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Search ID</p></td>
<td><p>Displays the Search ID for the page. The Search ID is the table containing the index used for search.</p>
<p>Search ID is the ID of a predefined Search set. They are defined in the Admin &gt; Data Sources &gt; Index icon &gt; <em><a href="Index%20Specification%20H">Index (Specification)</a></em> page.</p>
<p>See <a href="../Use_Cases/Create%20an%20Index">Create an Index</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Duplicate Detection Search ID</p></td>
<td><p>Displays the Duplicate Detection Search ID for the page. The Duplicate Detection Search ID is the table containing the index used for bulk duplicate detection.</p>
<p>Duplicate Detection Search ID is the ID of a predefined search set to use when looking for duplicates. They are defined in the Admin &gt; Data Sources &gt; Index icon &gt; <em><a href="Index%20Specification%20H">Index (Specification)</a></em> page.</p>
<p>A page may use different searches for regular searching and duplicate detection. For instance, you may allow users to search the customer table by both name and street address, but when detecting duplicates, you may want to restrict the search to name only.</p>
<p>See <a href="../Use_Cases/Build%20Indices%20for%20a%20Data%20Source%20for%20Search%20and%20Duplicate%20Detection">Build Indices for a Data Source for Search and Duplicate Detection</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Duplicate Detection Binding Field Names</p></td>
<td><p>Displays the Binding Fields used for Bulk Duplicate Detection for the page.</p>
<p>This field is similar to the Binding Fields when defining a Link To another page on a column.</p>
<p>By default the DSP® joins the page's view to the page's duplicate detection table using primary keys. It is possible to override this default and use custom joining fields by configuring this setting (for example, TableColumnName=IndexColumnName). This feature is typically used when using a Request page, but enabling search against an SAP data set. The Duplicate Detection process checks against a different table than the current page's table to avoid duplicating data in the target.</p>
<p>See <a href="../Use_Cases/Build%20Indices%20for%20a%20Data%20Source%20for%20Search%20and%20Duplicate%20Detection">Build Indices for a Data Source for Search and Duplicate Detection</a> for more information.</p></td>
</tr>
</tbody>
</table>

## <span id="DynamicDepPropstab"></span>Dynamic Page Type: Deprecated Properties tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Support Full Page Update</p></td>
<td><p>If checked, records on the <em>Horizontal</em> View of the page can be edited. If unchecked, editing for a record can only be performed on the <em>Vertical</em> View.</p></td>
</tr>
<tr class="odd">
<td><p>Horizontal Titlebar</p></td>
<td><p>Displays the column name of the page's underlying table or view containing the data that displays in the title bar on the <em>Horizontal</em> view.</p></td>
</tr>
<tr class="even">
<td><p>Vertical Titlebar</p></td>
<td><p>Displays the column name of the page's underlying table or view containing the data that displays in the title bar on the <em>Vertical</em> view.</p></td>
</tr>
<tr class="odd">
<td><p>Default Page Mode</p></td>
<td><p>Displays how pages are initially displayed when records can be added on the page but no records have been added yet.</p>
<p>Options are:</p>
<ul>
<li><strong>Display</strong> — The user must use buttons to add and edit records on the page, even if no records exist.</li>
<li><strong>Insert</strong> — The page displays in Add mode, ready to accept data without the user having to select an Add or Edit button. The Save button is active.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Breadcrumb Alias Horizontal</p></td>
<td><p>Contains an alias for the Horizontal View of the page that displays in the breadcrumbs.</p></td>
</tr>
<tr class="odd">
<td><p>Breadcrumb Alias Vertical</p></td>
<td><p>Contains an alias for the <em>Vertical</em> View of the page that displays in the breadcrumbs.</p></td>
</tr>
</tbody>
</table>

## <span id="Static"></span>Static Page Type V (All tabs)

This page contains the following tabs:

  - [General tab](#StaticGentab)
  - [Advanced Properties tab](#StaticAdvPropstab)

<div class="use">

Use this page to [Create a Static
Page.](../../WebApp_Dev/Create%20a%20Static%20Page)

</div>

## <span id="StaticGentab"></span>Static Page Type: General tab

Field

Description

Description

Displays the page name.

Page Type

Displays the page type, in this case Static.

Basic Properties

Static Source

Displays the text that displays on the page.

Horizontal Menu ID

Displays the name of the menu that displays in the *Navigation* pane
when the page is accessed. The standard menu is {component name} :
Switchboard.

Vertical Menu ID

This field is not
used.

## <span id="StaticAdvPropstab"></span>Static Page Type: Advanced Properties tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Short Description</p></td>
<td><p>Displays a short description of the page for documentation purposes only.</p></td>
</tr>
<tr class="odd">
<td><p>Refresh Rate</p></td>
<td><p>Displays the amount of time in seconds that passes before the page is automatically refreshed. If the value is 0, the page is not automatically refreshed.</p></td>
</tr>
<tr class="even">
<td><p>Allow Explicit Quick Link</p></td>
<td><p>If checked, this page can be linked to using the Quick Links feature. Refer to <a href="../Use_Cases/Quick_Links">Quick Links</a> for more information.</p>
<p>If this page requires binding to function correctly (Page Control View for example) then this setting must be unchecked.</p></td>
</tr>
<tr class="odd">
<td><p>Catalog ID</p></td>
<td><p>Displays the name of the catalog used for translations for this page, if needed.</p>
<p>Refer to <a href="../Use_Cases/Manage_Catalogs">Manage Catalogs</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Static Source as Full Screen</p></td>
<td><p>This field is not used.</p></td>
</tr>
<tr class="odd">
<td><p>Copy</p></td>
<td><p>Click to open the <em><a href="Copy%20Page">Copy Page</a></em> page to create a copy of the selected page to use as a basis for a new page. When a page is copied, the column properties, events, validations and other settings are copied.</p>
<p><strong>NOTE:</strong> This button is disabled if the page is in Edit mode.</p>
<p>Refer to <a href="../../WebApp_Dev/Copy_a_Page_in_a_WebApp">Copy a Page in a WebApp</a> for more information.</p></td>
</tr>
</tbody>
</table>

## <span id="Header"></span>Header Detail Page Type V (All tabs)

This page contains the following tabs:

  - [General tab](#HeaderDetGentab)
  - [Advanced Properties tab](#HeaderDetAdvPropstab)

<div class="use">

Use this page to [Create a Header Detail
Page](../../WebApp_Dev/Create_Header_Detail_Pages).

</div>

## <span id="HeaderDetGentab"></span>Header Detail Page Type: General tab

|                    |                                                                                                                                                                                                                                                                      |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field              | Description                                                                                                                                                                                                                                                          |
| Description        | Displays the page name.                                                                                                                                                                                                                                              |
| Page Type          | Displays the page type, in this case Header Detail.                                                                                                                                                                                                                  |
| Default Partition  | Displays how the header detail pages open by default. If the partition is horizontal, the header page displays in the upper frame and the details page displays in the lower frame. If the partition is vertical, that header and detail pages display side by side. |
| Frames             | Click the icon to open the *[Layout Frames](Layout%20Frames)* page to set the pages that are used for the Header and Detail pages.                                                                                                                               |
| Horizontal Menu ID | Displays the name of the menu that displays in the *Navigation* pane when the page is accessed. The standard menu is {component name} : Switchboard.                                                                                                                 |
| Vertical Menu ID   | This field is not used.                                                                                                                                                                                                                                              |

## <span id="HeaderDetAdvPropstab"></span>Header Detail Page Type: Advanced Properties tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Short Description</p></td>
<td><p>Displays a short description of the page.</p></td>
</tr>
<tr class="odd">
<td><p>Allow Explicit Quick Link</p></td>
<td><p>If checked, this page can be linked to using the Quick Links feature. Refer to <a href="../Use_Cases/Quick_Links">Quick Links</a> for more information.</p>
<p>If this page requires binding to function correctly (Page Control View for example) then this setting must be unchecked.</p></td>
</tr>
<tr class="even">
<td><p>Copy</p></td>
<td><p>Click to open the <em><a href="Copy%20Page">Copy Page</a></em> page to create a copy of the selected page to use as a basis for a new page. When a page is copied, the column properties, events, validations and other settings are copied.</p>
<p><strong>NOTE:</strong> This button is disabled if the page is in Edit mode.</p>
<p>Refer to <a href="../../WebApp_Dev/Copy_a_Page_in_a_WebApp">Copy a Page in a WebApp</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Page Title</p></td>
<td><p>Displays the title for the header detail page, which is the [component name]: [page name].</p></td>
</tr>
<tr class="even">
<td><p>Mode</p></td>
<td><p>This field is not used.</p></td>
</tr>
</tbody>
</table>

## <span id="Chart"></span>Chart Page Type V (All tabs)

This page contains the following tabs:

  - [General tab](#ChartGentab)
  - [Advanced Properties tab](#ChartAdvPropstab)

<div class="use">

Use this page to [Create a Chart](../../WebApp_Dev/Create_a_Chart).

</div>

## <span id="ChartGentab"></span>Chart Page Type: General tab

Field

Description

Description

Displays the page name.

Page Type

Displays the page type, in this case Chart.

Basic Properties

Report View

Displays the name of the SQL view upon which the chart is based.

Horizontal Menu ID

Displays the name of the menu that displays in the *Navigation* pane
when the page is accessed. The standard menu is {component name} :
Switchboard.

Vertical Menu ID

This field is not used.

Chart Type

Displays the type of chart, such as Bar or Line.

Chart Properties

Click to open the *[Page (Chart
Properties)](Page%20Chart%20Properties)* page to set properties for
the chart page, such as the location of the legend and labels, whether
data displays in a hover view and other options.

Refer to [Modify a Chart](../../WebApp_Dev/Modify_Chart_Properties)
for more
information.

## <span id="ChartAdvPropstab"></span>Chart Page Type: Advanced Properties tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Short Description</p></td>
<td><p>Displays a short description of the page for documentation purposes only.</p></td>
</tr>
<tr class="odd">
<td><p>Order By</p></td>
<td><p>Displays the field to sort by. Sorting must be done in the DSP®, not in the SQL view.</p>
<p>For example, a bar chart with labels can be sorted by the field that contains the label names. The bars would appear in that order when the chart displays.</p>
<p><strong>NOTE:</strong> When a field name is entered in Order By field, the default order is ascending. To sort in descending order, enter the field name followed by a space and desc, for example, lastname desc. Separate entries by a comma.</p></td>
</tr>
<tr class="even">
<td><p>Refresh Rate</p></td>
<td><p>Displays the amount of time in seconds that passes before the page is automatically refreshed. If the value is 0, the page is not automatically refreshed.</p></td>
</tr>
<tr class="odd">
<td><p>Static Source</p></td>
<td><p>This field is not used.</p></td>
</tr>
<tr class="even">
<td><p>Catalog ID</p></td>
<td><p>Displays the name of the catalog used for translations for this page, if needed.</p>
<p>Refer to <a href="../Use_Cases/Manage_Catalogs">Manage Catalogs</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Allow Explicit Quick Link</p></td>
<td><p>If checked, this page can be linked to using the Quick Links feature. Refer to <a href="../Use_Cases/Quick_Links">Quick Links</a> for more information.</p>
<p>If this page requires binding to function correctly (Page Control View for example) then this setting must be unchecked.</p></td>
</tr>
<tr class="even">
<td><p>Ver Title</p></td>
<td><p>This field is not used.</p></td>
</tr>
<tr class="odd">
<td><p>Title Bar</p></td>
<td><p>This field is not used.</p></td>
</tr>
<tr class="even">
<td><p>Copy</p></td>
<td><p>Click to open the <a href="Copy%20Page">Copy Page</a> page to create a copy of the selected page to use as a basis for a new page. When a page is copied, the column properties, events, validations and other settings are copied.</p>
<p><strong>NOTE:</strong> This button is disabled if the page is in Edit mode.</p>
<p>Refer to <a href="../../WebApp_Dev/Copy_a_Page_in_a_WebApp">Copy a Page in a WebApp</a> for more information.</p></td>
</tr>
</tbody>
</table>

## <span id="Dashboar"></span>Dashboard Page Type V (All tabs)

This page contains the following tabs:

  - [General tab](#DashboardGentab)
  - [Advanced Properties tab](#DashboardAdvPropstab)

<div class="use">

Use this page to [Create a
Dashboard](../../WebApp_Dev/Create_a_Dashboard).

</div>

## <span id="DashboardGentab"></span>Dashboard Page Type: General tab

Field

Description

Description

Displays the page name.

Page Type

Displays the page type, in this case Dashboard.

Layout ID

Displays the layout that is used for the dashboard. Layouts that are
installed with the platform can be viewed on the
*[Layouts](Layouts)* page. A user can also add a layout. Refer to
[Create a Dashboard](../../WebApp_Dev/Create_a_Dashboard) for more
information.

Basic Properties

Horizontal Menu ID

Displays the name of the menu that displays in the *Navigation* pane
when the page is accessed. The standard menu is {component name} :
Switchboard.

Vertical Menu ID

This field is not
used.

## <span id="DashboardAdvPropstab"></span>Dashboard Page Type: Advanced Properties tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Short Description</p></td>
<td><p>Displays a short description of the page for documentation purposes only.</p></td>
</tr>
<tr class="odd">
<td><p>Catalog ID</p></td>
<td><p>Displays the name of the catalog used for translations for this page, if needed.</p>
<p>Refer to <a href="../Use_Cases/Manage_Catalogs">Manage Catalogs</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Allow Explicit Quick Link</p></td>
<td><p>If checked, this page can be linked to using the Quick Links feature. Refer to <a href="../Use_Cases/Quick_Links">Quick Links</a> for more information.</p>
<p>If this page requires binding to function correctly (Page Control View for example), then this setting must be unchecked.</p></td>
</tr>
<tr class="odd">
<td><p>Ver Title</p></td>
<td><p>This field is not used.</p></td>
</tr>
<tr class="even">
<td><p>Titlebar</p></td>
<td><p>This field is not used.</p></td>
</tr>
<tr class="odd">
<td><p>Copy</p></td>
<td><p>Click to open the <em><a href="Copy%20Page">Copy Page</a></em> page to create a copy of the selected page to use as a basis for a new page. When a page is copied, the column properties, events, validations and other settings are copied.</p>
<p><strong>NOTE:</strong> This button is disabled if the page is in Edit mode.</p>
<p>Refer to <a href="../../WebApp_Dev/Copy_a_Page_in_a_WebApp">Copy a Page in a WebApp</a> for more information.</p></td>
</tr>
</tbody>
</table>

## <span id="Service"></span>Service Page V (All tabs)

This page contains the following tabs:

  - [General tab](#ServiceGentab)
  - [Advanced Properties tab](#ServiceAdvPropstab)

<div class="use">

Use this page to [create a Service
page](../../WebApp_Dev/Create%20a%20Service%20Page).

</div>

## <span id="ServiceGentab"></span>Service Page Type: General tab

Field

Description

Description

Displays the page name.

Page Type

Displays the type of page, in this case, Service.

Basic Properties

Table

Displays the table where the data for the page is stored.

Horizontal View

Displays the name of the Horizontal View that contains the list of
records that the service page must execute on. If there are no records
in the view, the service page does not
run.

## <span id="ServiceAdvPropstab"></span>Service Page Type: Service Properties tab

<table>
<tbody>
<tr class="odd">
<td><p>Fields</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Queue ID</p></td>
<td><p>Displays the queue ID that determines which Service Queue is used during execution. This can be used to serialize certain operations or load balance.</p></td>
</tr>
<tr class="odd">
<td><p>Next Service Date</p></td>
<td><p>Displays the next service date and time the service page will run.</p></td>
</tr>
<tr class="even">
<td><p>Service Qty</p></td>
<td><p>Displays the frequency that the service page will run and used in conjunction with the UOM (Unit of Measure) field. For example, if the Service Qty field displays 2 and the Service UOM field is Day(s) the service page runs every two days starting from the date displayed in the Next Service Date field.</p></td>
</tr>
<tr class="odd">
<td><p>Service UOM</p></td>
<td><p>Displays the service UOM (Unit of Measure) that is used in conjunction with the number in the Service Qty field to set the frequency that the service page will run.</p></td>
</tr>
<tr class="even">
<td><p>Active</p></td>
<td><p>If checked, the service page will run. If unchecked, the service page will not run but can be activated at a later date to run again. .</p></td>
</tr>
<tr class="odd">
<td><p>Copy</p></td>
<td><p>Click to open the <em><a href="Copy%20Page">Copy Page</a></em> page to create a copy of the selected page to use as a basis for a new page. When a page is copied, the column properties, events, validations and other settings are copied.</p>
<p><strong>NOTE:</strong> This button is disabled if the page is in Edit mode.</p>
<p>Refer to <a href="../../WebApp_Dev/Copy_a_Page_in_a_WebApp">Copy a Page in a WebApp</a> for more information.</p></td>
</tr>
</tbody>
</table>

## <span id="Report"></span>Report Page V (All tabs)

This page contains the following tabs:

  - [General tab](#ReportGentab)
  - [Advanced Properties tab](#ReportAdvPropstab)

<div class="use">

Use this page to [Create a Report
Page](../../WebApp_Dev/Create%20a%20Service%20Page).

</div>

## <span id="ReportGentab"></span>Report Page Type: General tab

Field

Description

Description

Displays the page name.

Page Type

Displays the type of page, in this case, Report.

Basic Properties

Report View

Displays the view used to generate report.

Order By

Displays a SQL Order By clause used to sort the page.

**NOTE:** Do not include "ORDER BY" in the clause

Priority

Displays the order the reports are listed on the page.

Report Groups

Displays the Report Groups used to customize the layout of the report.

Horizontal Menu ID

Displays the name of the horizontal menu. If left blank, the horizontal
menu is not used for this page.

Vertical Menu ID

This field is not
used.

## <span id="ReportAdvPropstab"></span>Report Page Type: Advanced Properties tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Short Description</p></td>
<td><p>Displays a short description of the page for documentation purposes only.</p></td>
</tr>
<tr class="odd">
<td><p>Allow Explicit Quick Link</p></td>
<td><p>If checked, this page can be linked to using the Quick Links feature. Refer to <a href="../Use_Cases/Quick_Links">Quick Links</a> for more information.</p>
<p>If this page requires binding to function correctly (Page Control View for example), then this setting must be unchecked.</p></td>
</tr>
</tbody>
</table>
