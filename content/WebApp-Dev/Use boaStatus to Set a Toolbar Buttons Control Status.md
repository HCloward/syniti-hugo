# Use boaStatus to Set a Toolbar Button's Control Status

Refer to [Add a Toolbar
Button](../Sys_Admin/Use_Cases/Add%20a%20Toolbar%20Button.htm) for
general information.

A toolbar button can be made active or dimmed depending on a selected
record’s boaStatus value.

When the Consider Valid check box is checked for the toolbar button on
the *[Page Columns](../Sys_Admin/Page_Desc/Page_Columns_H.htm)* page’s
*Vertical* View, the DSP® uses a record’s boaStatus value to set the
button to active. By default, if a record‘s boaStatus is Validation
Passed or Procedure Complete, the toolbar button is active. If the
record is in any other boaStatus, the toolbar button is dimmed when the
user selects that record.

On the *[Status](../Sys_Admin/Page_Desc/Status.htm)* page, the boaStatus
values with the CONSIDER VALID check box checked return 1 (enabled). By
default, these statuses are 3 (Validation Passed) and 4 (Procedures
Completed).

A user can also set another column in the view that dictates whether the
control is enabled, disabled, or hidden, instead of using the currently
selected column or boaStatus to determine control status. Refer to [Set
Column Control Status](Set_Column_Control_Status.htm) for more
information.
