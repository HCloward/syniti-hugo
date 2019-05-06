# Add List Boxes and Combo Boxes

List box and combo box are Control Types that display a field as a list
box or text box with options from a selected table or view.

When creating list views:

  - Use the naming convention **webXXXList** where **XXX** describes
    what is being listed, for example, webProductList.
  - Include only the columns that apply to the List Value, List Display,
    List Select or List WHERE clause registrations.
  - Include a unique set of data.
  - Do not sort in the view. Sorting is done in DSP® using the List
    Order By Column Property option. Sorting is not officially supported
    in later versions of Microsoft SQL Server.

When creating a combo box:

  - Only values in the list view can be entered in the field.

  - Use a combo box instead of a list box when the list view contains
    too many records to display suitably as a List Box.

  - Enable List Filter to allow filter on a combo box.

  - Include both a description field and a combined value and
    description field. Do not display both on the combo box filter page
    to prevent displaying duplicate field information. You can hide
    either of the fields using a column property with View Type set to
    Filter (Control) and selecting hide in the Control Status property.
    If the list view contains other fields that do not aid in the combo
    box search, you can hide them using additional Filter (Control)
    properties.

  - Create a column property with View Type set to Control to define the
    list view properties for fields which have check tables.

To create a list box or combo box:

1.  <span id="Column Properties Navigation" class="popUpLink">Access the
    *Page Columns* page</span>.

2.  Click **Add**.
    
    *[View the field descriptions for the Page Columns
    page](../Sys_Admin/Page_Desc/Page_Columns_H.htm)*

3.  Enter the name of the list box or combo box in the **COLUMN** field.

4.  Select **List Box** or **Combo Box** in the **CONTROL** list box.

5.  Select the list box or combo box view from the **LIST SOURCE** list
    box.

6.  Click **Save**.

7.  Click **Vertical View**.

8.  Select the value that stores the field from the**List Value Field**
    list box.

9.  Select the field that displays a description of the field from
    the**List DisplayField** list box.
    
    **NOTE:** In most cases, List Value Field is the primary key stored
    in the table and List Display Field is the option visible in the
    list box.

10. Click **Save**.

These settings are available for List Boxes and Combo Boxes:

  - [Enable List Unique](Enable_List_Unique.htm)
  - [Enable List Allow Insert](Enable_List_Allow_Insert.htm)
  - [Enable List Where Clause](Enable_List_Where_Clause.htm)
  - [Add a List Selection Field](Add_a_List_Selection_Field.htm)
  - [Set the List Order By](Set_the_List_Order_By.htm)
  - [Set a Dynamic List Box](Set_a_Dynamic_List_Box.htm)
  - [Add a Filtered Combo Box](Add_a_Filtered_Combo_Box.htm)
