+++
title = 'Use View Types with Column Properties'
solution = 'Platform'
+++

# Use View Types with Column Properties

The View Type sets the context in which the control is configured for a
column. Multiple records for a column can be added on the *[Page
Columns](../Sys_Admin/Page_Desc/Page_Columns_H.htm)* page, each having a
different view type.

When adding a column, the View Type of All Views can be used in most
cases. However, column properties can be applied to other views as
needed. For example, a field can be a Combo Box on the *Horizontal*
View, but can be a display-only field on the *Vertical* View. In this
case, set the field as a Combo Box for the View Type of All Views. Add
another record for the field and select a View Type of Vertical, and set
the CONTROL STATUS to Disabled.

Refer to [Set Column Control Status](Set_Column_Control_Status.htm) for
more information.

View Types are:

  - **All Views —** The column properties set for All View are applied
    to all other View Types by default, but can be overwritten by
    properties set for other View Types. For example, If a column is
    hidden for All Views, but enabled for Download, the column does not
    display for any other View Type, but does display when the page is
    downloaded.
  - **Download —** The column property is configured for the Download
    panel, accessible when the user clicks the gear on the Page toolbar
    and selects Download. Refer to [Hide a Column from
    Download](Hide%20a%20Column%20from%20Download.htm) for more
    information.
  - **Excel —** This setting allows columns to be included or excluded
    from the spreadsheet downloaded for Excel Integration. Refer to
    [Exclude Columns from Excel
    Integration](../Sys_Admin/Use_Cases/Exclude%20Columns%20Excel%20Integration.htm)
    for more information.
  - **Filter (Control) —** This setting allows for manipulation of a
    column property within the Combo Box Filter form, accessible when
    the user clicks the Goggles next to a Combo Box field. The Goggles
    appear only in edit mode and only on Combo Boxes with the List
    Filter property enabled.
  - **Filter (Form) —** This setting allows for manipulation of a column
    property within the Filter form, accessible when the user clicks the
    Gear on the Page toolbar and selects Filter. Refer to [Hide Columns
    on a Page’s Filter
    View](../Sys_Admin/Use_Cases/Hide%20Columns%20on%20a%20Pages%20Filter%20View.htm)
    and [Display Fields as List Boxes on a Page’s Filter
    View](../Sys_Admin/Use_Cases/Display%20Fields%20as%20List%20Boxes%20on%20a%20Pages%20Filter%20View.htm)
    for more information.
  - **Horizontal —** The column property applies to the *Horizontal*
    View only.
  - **Print —** This option is not used.
  - **Report —** This column property applies to reports, accessible
    when the user clicks the gear on the Page toolbar and selects
    Report. Refer to [Hide a Page Column on a
    Report](Hide%20a%20Page%20Column%20on%20a%20Report.htm) for more
    information.
  - **Vertical —** The column property applies to the *Vertical* View
    only.
