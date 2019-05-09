+++
title = 'Add a Toolbar Button'
solution = 'Platform'
+++

# Add a Toolbar Button

A toolbar displays at the top of the page, and contains buttons that can
be used for page navigation, to link to additional pages or to perform
some action, such as run a rule.

After a toolbar control has been added for a column, a toolbar button is
added to the toolbar.

**NOTE:** A NULL column with an alias must be added to the underlying
view to add a Toolbar button to a column that does not contain data. The
view must be modified in SQL before the Toolbar button can be added.

**NOTE:** The DSP® can pass binding criteria to the *Linked To* page to
display data relevant for that selected record. If binding criteria is
not specified, the *Linked To* page binds on like primary keys. If the
primary keys are different, the *Linked To* page displays all records.
Refer to [Add Binding Criteria when Linking to a
Page](../../WebApp_Dev/Add%20Binding%20Criteria%20when%20Linking%20to%20a%20Page)
for more information.

To add a Toolbar button in DSP Application Development:

1.  Navigate to the
    <span id="Column Properties Navigation" class="popUpLink">*Page
    Columns*</span> page’s *Vertical* View for the column with the
    Toolbar control. and click **Edit**.
    
    *[View the field descriptions for the Page Columns
    page](../Page_Desc/Page_Columns_H)*

2.  Select the button image from the **Image ID** list box.

3.  Select the page to open when the toolbar button is clicked from the
    **Link to Page ID** list box.

4.  Click the **Advanced Properties** tab.

5.  Select an option in the **Dynamic Link Type** list box.
    
    **NOTE:** This option determines if the link is to a page, a view,
    or a URL.

6.  Select an option in the **Link to Method** list box.
    
    **NOTE:** This option sets whether the page that is accessed from
    the toolbar button overlays the existing page, or opens in a
    separate page.

7.  Click the **Consider Valid** check box.
    
    **NOTE:** If checked, the platform uses the boaStatus column to
    determine whether the control (in this case, the toolbar button) is
    active or dimmed. Refer to [Use boaStatus to Set a Toolbar Button’s
    Control
    Status](../../WebApp_Dev/Use%20boaStatus%20to%20Set%20a%20Toolbar%20Buttons%20Control%20Status)
    for more information.

8.  Click the **Allow Multi Row Action** check box.
    
    **NOTE:** If checked, a user can select multiple records on the
    *Horizontal* View and click the toolbar button to perform the action
    related to the toolbar button on multiple records at once.

9.  Click **Save**.
