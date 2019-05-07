+++
title = 'Set Column Control Status'
solution = 'Platform'
+++

# Set Column Control Status

Control Status is a Column Property option that determines the
visibility of a column on a page. Options are:

  - **Enabled** – Displays the column on the page. This is the default
    value.
  - **Hide** – Hides the column on the page.
  - **Disabled** – Protects the column. Displays as read-only columns
    when in edit mode.

**NOTE:** Control status cannot be set for columns using tab or label
controls.

Control Status can be set:

  - [As a property of the column](#To_set_a_column’s_Control_Status:%0A)
  - Using the boaStatus value. Refer to [Use boaStatus to Set a Toolbar
    Button’s Control
    Status](Use%20boaStatus%20to%20Set%20a%20Toolbar%20Buttons%20Control%20Status.htm)
  - [Using the value from another
    field](#o_set_Control_Status_for_the_column_using_the_value)

A column’s control status may be set differently for different views.
For example, a column that stores a user comment may be hidden on the
*Horizontal* View, but enabled on the *Vertical* View.

<span id="To_set_a_column’s_Control_Status:
"></span>To set a column’s Control Status as a column property in
DSP Application Development:

1.  <span id="Column Properties Navigation" class="popUpLink">Navigate
    to the *Page Columns* page.</span>

2.  Click **Edit** for the column.
    
    *[View the field descriptions for the Page Columns
    page](../Sys_Admin/Page_Desc/Page_Columns_H.htm)*

3.  Select **Hide**, **Disabled**, or **Enabled** from the **CONTROL
    STATUS** list box.

4.  Click **Save**.

<span id="o_set_Control_Status_for_the_column_using_the_value"></span>To
set Control Status for the column using the values from another bit
field in DSP Application Development:

1.  Navigate to the *Page Columns* page.

2.  Click **Vertical View** for the column.

3.  Click the **Enable/Disable Control** tab.

4.  Click **Edit**.

5.  Leave the **Consider Valid** check box unchecked.

6.  Select the field from the page’s underlying table to be used to set
    the Control Status from the **Control Status Field** list box. ;
    
    **NOTE:** This field must be a bit field.

7.  Click **Save**.
