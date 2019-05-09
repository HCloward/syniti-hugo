+++
title = 'Page Column Links'
solution = 'Platform'
+++

# Page Column Links

<div class="use">

Use this page to [Add Binding Criteria when Linking to a
Page](../../WebApp_Dev/Add%20Binding%20Criteria%20when%20Linking%20to%20a%20Page).

</div>

To access this page:

1.  <span id="Column Properties Navigation" class="popUpLink">Navigate
    to the Page Columns page.</span>
2.  Click the link in the **LINK TO PAGE** column.

This page contains the following tabs:

  - [General](#General)
  - [Advanced Properties](#Advanced)

### <span id="General"></span>General tab

Field

Description

Data Options

Binding Field Names

Displays a comma-separated list of columns used to filter data on a
linked page. By default, when linking from one page to another, the DSP®
sends the key field(s) to the linked page. However, if the key field(s)
are different between linked pages, use this field to indicate the
columns.

For instance, a user clicks a button on a *Country* page listing country
records to access a *Region* page listing the selected country’s
regions. If the Country field does not have the same name on both pages,
the field on the linked page (the *Country* page) must be included as
part of the binding criteria. Otherwise, the *Region* page displays
regions for all countries.

Shared Field Names

Displays a comma-separated list of columns used to send data to a linked
page.

Shared Fields tell the DSP® to send the data from a column that is not
normally passed and allow it to be used on a subsequent page. For
example, to filter a Region list box on the *Region* page by the Country
field that was entered on the *Country* page, add the Country field as a
Shared Field on the link between pages. It is then available for use in
the list box Where Clause on the *Region* page.

If the Country field is set as a Shared Field and not a Binding Field,
the linked to page (the *Region* page) displays regions for all
countries, but any list boxes with a Country filter display regions
filtered by the country shared from the *Country* page.

Report Options

Report Follows Link

If checked, generates a report for the current Dynamic page for the
*Horizontal* or *Vertical* Views.

Refer to [Include all Page Details in
Reports](../../WebApp_Dev/Include_All_Page_Details_in_Reports) for
more information.

Link to Report

If checked, when a user clicks the image, the page to access opens in a
read-only format.

By default, page links render data using the normal *Horizontal* or
*Vertical* View with add/edit/delete capability. Link to Report provides
a mechanism to report data as read-only without having to modify
defaulted page properties.

Refer to [Link to a Report from a
Page](../../WebApp_Dev/Link_to_a_Report_from_a_Page) for more
information.

### <span id="Advanced"></span>Advanced Properties tab

Field

Description

Display Null As Zero

If checked, if the binding field does not contain data, it displays 0 on
the Linked to page.

Inherit Validations

If checked, any validations on the current page run on the linked to
page as well. Refer to [Enable Inherit
Validations](../../WebApp_Dev/ValidationRules) for more information.

Invoke On Insert

If checked, the link is automatically invoked when a user adds a new
record on the page.

**NOTE:** If this setting is checked for multiple links on a page, only
the first link is invoked when a record is added.

Link Tag

Displays the identifying string to pass to the Linked To page.

This feature supports child pages that require different
PageControlViews depending on which parent page they are being linked to
from.

For example, a child page is registered with a PageControlView of the
form ”webMyTable\#LinkTag\#Pcv.”

The page Designer builds parent-specific views for two parent pages. The
view names are ”webMyTable\#OneParent\#Pcv” and
”webMyTable\#OtherParent\#Pcv.”

Then, for the buttons that link to the child page from each parent page,
the Designer sets the Link Tag properties accordingly. In this example,
"OneParent" and "OtherParent" would be entered as the Link Tag for the
buttons on the different parent pages

Link To Method

Displays how the linked to page opens. Options are:

  - **Overwrite Layout Pages** — Opens the link in the current window,
    replacing the current page.
  - **Popup Window** — Opens the link in a new window or tab, depending
    on the browser settings.

Advanced Data Options

Select Field Names

This field is not used.

Deprecated Properties

Link to Page Mode

This field is not used.

Link To Page Mode Control

This field is not used.
