+++
title = 'Set the List Order By'
solution = 'Platform'
+++

# Set the List Order By

By default, like pages, list boxes are sorted based on the primary key.
Use List Order By to sort select options in a list box based on another
field.

**NOTE:** DSP® and SQL Server no longer support the sort in a view in
SQL.

Refer to [Add List Boxes and Combo
Boxes](Add_List_Boxes_and_Combo_Boxes.htm) for general information.

To order the list box options:

1.  <span id="Column Properties Navigation" class="popUpLink">Access the
    *Page Columns* page</span> *Vertical* View for a list box or combo
    box.

2.  Click **Edit**.
    
    *[View the field descriptions for the Page Columns
    page](../Sys_Admin/Page_Desc/Page_Columns_H.htm)*

3.  Click the **Advanced Properties** tab.

4.  Enter the column that should sort n **List Order By** field.

5.  Click **Save**.

**NOTE:** When a field name is entered in **ListOrder By** field, the
default order is ascending. To sort in descending order, enter the field
name followed by a space and **desc**, for example, **ProductName
desc**. Separate entries by a comma.
