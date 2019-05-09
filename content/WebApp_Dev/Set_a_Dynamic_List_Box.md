+++
title = 'Set a Dynamic List Box'
solution = 'Platform'
+++

# Set a Dynamic List Box

Dynamic List Box is a feature that uses a Where Clause to control the
values displayed in one list box based on the value selected from
another list box. Dynamic List Boxes can be used for list boxes on the
same page view.

For example, a user could add a list box and create a Where Clause on
the State field on the *Customers* page so the country selected
determines the values displayed in the States/Regions list box.

Refer to [Add List Boxes and Combo
Boxes](Add_List_Boxes_and_Combo_Boxes) for general information.

To filter the options in one list box based on the value selected from
another on the same view:

1.  <span id="Column Properties Navigation" class="popUpLink">Access the
    *Page Columns* page</span>.

2.  Click **Add**.
    
    *[View the field descriptions for the Page Columns
    page](../Sys_Admin/Page_Desc/Page_Columns_H)*

3.  Enter the name of the list box or combo box in the **COLUMN** field.

4.  Select **List Box** or **Combo Box** in the **CONTROL** list box.

5.  Select the List Box or Combo Box view from the **LIST SOURCE** list
    box.

6.  Click **Save**.

7.  Click **Vertical View**.

8.  Select the view from the database that provides the values to the
    list box from the **List Source** list box.

9.  Select the name of the column that will be stored from the **List
    Value Field** list box.

10. Select the name of the column that displays a description of the
    item from the **List Display Field** list box.

11. Click **Save**.

To create a WHERE clause that controls the options in a list box based
on a value selected from another list box for the same page view:

1.  Click the **Advanced Properties** tab on the *Page Columns* page's
    *Vertical* View.

2.  Enter the WHERE clause in the **List Where Clause** field.
    
    **NOTE:** For example, a user can filter the Region List Box by
    Country by entering CountryID = N’\#Country’. If the Country field
    contains text, single quotes are required to indicate the field
    contains text and N is required to indicate the text field contains
    Unicode characters. If the N is excluded, Unicode characters will be
    lost. The field name to the left of the operator is the field name
    in the list view. The field name to the right of the operator is
    being passed in from the page. Surrounding the column name with
    pound signs (\#) indicates it is a dynamic field and the value is
    coming from the page view. If the field is numeric, the N and the
    single quotes must be excluded. For example, if the CountryID field
    is an integer data type in SQL, the Where Clause would be Country =
    \#CountryID\#.

3.  Click **Save**.
