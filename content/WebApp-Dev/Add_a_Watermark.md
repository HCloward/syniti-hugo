+++
title = 'Add a Watermark'
solution = 'Platform'
+++

# Add a Watermark

Some columns benefit from a watermark, which displays as grey text in
the field.

A watermark can be added in two ways: A static text watermark can be
added to a column, or a view can be registered that displays the
watermark depending on certain conditions.

For example, for list boxes that search for particularly named
values/objects a watermark can display the expected formats to ensure
that the user understands what’s expected. Also, suggested text formats
can be useful. If the user is expected to use a namespace convention,
indicating it during the add/edit is more useful than providing a
warning after the save.

A watermark can be added to these controls:

  - HTML Area
  - Text Box
  - DateTime
  - Combo Box
  - Numeric
  - List Box
  - Text Area

To add a static text watermark to a column:

1.  <span id="Column Properties Navigation" class="popUpLink">Access the
    *Page Columns* page</span>'s *Vertical* View.

2.  Click **Edit**.
    
    *[View the field descriptions for the Page Columns
    page](../Sys_Admin/Page_Desc/Page_Columns_H.htm)*

3.  Enter the text in the **Watermark Text** field.

4.  Click **Save**.

To use a view to display a watermark:

1.  Write a view with a Dwv suffix and alias the column as boawatermark

2.  Access the Page Columns page's *Vertical* View.

3.  Click **Edit**.
    
    *[View the field descriptions for the Page Columns
    page](../Sys_Admin/Page_Desc/Page_Columns_H.htm)*

4.  Click the **Relational** tab.

5.  Select the view in the **Watermark View** list box.

6.  Enter the binding field name(s) in the **Watermark Binding Field
    Names** text box.
    
    **NOTE:** Include a comma between names.

7.  Click **Save**.
