+++
title = 'Enable List Where Clause'
solution = 'Platform'
+++

# Enable List Where Clause

Add a list Where Clause to restrict the values that display in a list
box or combo box.

Refer to [Add List Boxes and Combo
Boxes](Add_List_Boxes_and_Combo_Boxes.htm) for general information.

To create a List Where Clause:

1.  <span id="Column Properties Navigation" class="popUpLink">Access the
    *Page Columns* page</span> *Vertical* View for a list box or combo
    box.

2.  Click **Edit**.
    
    *[View the field descriptions for the Page Columns
    page](../Sys_Admin/Page_Desc/Page_Columns_H.htm)*

3.  Click the **Advanced Properties** tab.

4.  Enter the WHERE clause in the **List Where Clause** field.

5.  Click **Save**.

**NOTE:** For nvarchar and nchar database fields, the **N** must be
prepended to string literals in Where Clauses so Unicode characters will
not be lost and the value must have single quotes on either side. This
is unnecessary for numeric fields.
