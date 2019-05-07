+++
title = 'Link to a Page Using Buttons and Images'
solution = 'Platform'
+++

# Link to a Page Using Buttons and Images

The Link to Page ID column property allows the user to set the page that
opens when an end user clicks a control.

**NOTE:** The Link to Page setting is available with other control
types, such as text box and Date Time. When using the Link to Page
setting with control types other than image, button and toolbar, the
text in the field displays with an underline. Clicking the link opens
the page.

Link to Page can be used to complete the overall navigation of the
WebApp. Buttons and images can be added to columns and the Page toolbar
to use as page links. Use an existing column in a view, or a count, or a
NULL and assign an alias so a Button, Image or Toolbar column property
can be added to the page in the DSP®. Buttons can display text or a
counter to indicate the number of records on the linked page. Links also
control the display for a Layout page type which displays the parent
data in the parent pane and the dependent data in the child pane.

**NOTE:** It is recommended to implement the page links in column
properties prior to building additional page properties. Testing
additional properties on pages that have not been linked within the
WebApp cannot be performed during implementation, leaving possible
errors undiscovered until later.

**NOTE:** A NULL column with an alias must be added to the underlying
view to add a button or an image to a column that does not contain data.
The view must be modified before a link from a button can be added.

**NOTE:** The DSP® can pass binding criteria to the Linked To page to
display data relevant for that selected record. If binding criteria is
not specified, the Linked To page binds on like primary keys. If the
primary keys are different, the Linked To page displays all records.
Refer to [Add Binding Criteria when Linking to a
Page](Add%20Binding%20Criteria%20when%20Linking%20to%20a%20Page.htm) for
more information.

To assign a link from a button on a header page to a detail page:

1.  <span id="Column Properties Navigation" class="popUpLink">Access the
    *Page Columns* page</span>'s *Vertical* View for the column with the
    button or image control.

2.  Click **Edit**.
    
    *[View the field descriptions for the Page Columns
    page](../Sys_Admin/Page_Desc/Page_Columns_H.htm)*

3.  Select the image name from the **ImageID** list box.

4.  Select the detail page name from **Link to Page ID** list box.

5.  Click **Save**.

Toolbar buttons can be added to the Page toolbars. The buttons can be
used for page navigation, to link to additional pages or to run a rule.

Refer to [Add a Toolbar
Button](../Sys_Admin/Use_Cases/Add%20a%20Toolbar%20Button.htm) for more
information.
