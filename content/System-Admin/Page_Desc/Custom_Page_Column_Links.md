# Custom Page Column Links

<div class="use">

Use this page to [Add Custom Links to a
Page.](../Use_Cases/Add_a_Custom_Link.htm)

</div>

This page contains the following tabs:

  - [General tab](#General_Tab)

  - [Advanced Properties tab](#Advanced_Properties_tab)

To access this page:

1.  Select **Admin \> Customization \> WebApp
    Customization** from *Navigation* pane.

2.  Click **Custom Links**for a WEB APP NAME.

### <span id="General_Tab"></span>General tab

Field

Description

Column Name

Displays the column name that appears as the custom link.

Data Options

Binding Field Names

Displays binding criteria between a parent and a child page. If blank,
the primary key on the parent table automatically becomes the binding
field; the parent and child field names must match to bind. Use this
field when the linking relationship cannot be inferred because keys have
different names from parent to child pages. A user may specify one or
more *parent=child* pairs. If specifying more than one pair, separate
each pair with a comma. For example: *CustomerID=CustID*; or
*EmployeeID=EmployeeID, Department=DepartNo*. 

Shared Field Names

Displays  column values to pass to the linked-to page. These values will
be displayed on the page title bar. Possible uses are for Filter or List
Box WHERE clauses. A user may specify one or more field names or
*parent=child* pairs (if the child page expects a different field
name).If specifying more than one field or pair, separate each item with
a comma. For example: *CustomerID=CustID*; or*EmployeeID=EmployeeID,
Department=DepartNo*. 

Report Options

Report Follows Link

If enabled the linked-to page will be included as a sub-report for all
linked pages; i.e., nested reports. If disabled, a report is generated
for only the current page.

Link To Report

If enabled, the link will immediately run a Report on the linked-to
page, instead of linking the page. If disabled, the user is navigates to
the specified linked-to-page.

### <span id="Advanced_Properties_tab"></span>Advanced Properties tab

 

Field

Description

Link to Method

Displays the  method in which the link opens.  Options are:

  - Overwrite Layout Pages – Opens the link in the current window,
    thereby replacing the current page.

  - Popup Window – Opens the link in a new window or tab, depending on
    the browser settings.

Advanced Data Options

Select Field Names

*Feature is not used.*

Deprecated Properties

Link To Page Mode

*Feature is deprecated.*
