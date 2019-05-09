+++
title = 'Add a List Selection Field'
solution = 'Platform'
+++

# Add a List Selection Field

The List Selection Field is a feature that displays more descriptive
text in a list box or a combo box when in add or edit mode. To use this
feature, modify the view in SQL and update the List Selection Field in
DSP®.

For example, two fields, **ProductID** and **Description** must display
in the **ProductID** list box when in add or edit mode on the *Order
Details* page. The description should only be visible in display mode.
For both fields to display in the **Product ID** list box in edit mode,
add a column in the SQL list view to concatenate the two fields.

Refer to [Add List Boxes and Combo
Boxes](Add_List_Boxes_and_Combo_Boxes) for general information.

To choose a descriptive field:

1.  <span id="Column Properties Navigation" class="popUpLink">Access the
    *Page Columns* page</span> *Vertical* View for a list box or combo
    box.

2.  Click **Edit**.
    
    *[View the field descriptions for the Page Columns
    page](../Sys_Admin/Page_Desc/Page_Columns_H)*

3.  Click the **Advanced Properties** tab.

4.  Select the concatenated or more descriptive field created in the
    view from the **List Selection Field** list box.

5.  Click **Save**.
