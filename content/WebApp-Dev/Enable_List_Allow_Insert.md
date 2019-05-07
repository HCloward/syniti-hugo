+++
title = 'Enable List Allow Insert'
solution = 'Platform'
+++

# Enable List Allow Insert

List Allow Insert is a list box and combo box search mechanism if the
value stored in the field is known or additional values not available in
the list need to be added. If this property is enabled, the value
entered displays under the search box for the list box or combo box.
Click the value entered to use that value.

Options for List Allow Insert are:

  - **No** – Insert does not display and additional options cannot be
    added or searched.
  - **Yes** – Insert displays and
    **<span class="underline"><span style="color: #ff0000;">any</span></span>**
    additional option can be entered in the field regardless of the
    options available in the list box or combo box. The record is
    considered valid. The added value does
    **<span class="underline"><span style="color: #ff0000;">not</span></span>**
    become a future option in the table.
  - **Constrained to table** – A user can add a new entry by clicking
    **Use this Value**. A validation rule automatically runs to verify
    the entry is valid. This prevents undesirable data being added to
    the list table.

List Allow Insert Page ID is a column property that works in conjunction
with List Allow Insert. This feature permits additional values not
available in the list to be added to the associated list. If both are
enabled, clicking the icon opens a window containing the page associated
with the list. Enter the new options in the fields and the value is
available in the list box when adding new records.

**NOTE:** The current user must have security to add new records to the
page associated with the list.

Refer to [Add List Boxes and Combo
Boxes](Add_List_Boxes_and_Combo_Boxes.htm) for general information.

To enable List Allow Insert Page ID:

1.  <span id="Column Properties Navigation" class="popUpLink">Access the
    *Page Columns* page's</span> *Vertical* View for a list box or combo
    box.

2.  Click **Edit**.
    
    *[View the field descriptions for the Page Columns
    page](../Sys_Admin/Page_Desc/Page_Columns_H.htm)*

3.  Click the **Advanced Properties** tab.

4.  Select **Yes** from the **List Allow Insert** list box.
    
    **NOTE:** Yes must be selected so a new record can be added and
    validated.

5.  Select the page name from **List Allow Insert Page ID** list box.

6.  Click **Save**.
