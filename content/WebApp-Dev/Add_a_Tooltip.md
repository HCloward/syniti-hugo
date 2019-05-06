# Add a Tooltip

Some columns may benefit from a tooltip, such as images that represent a
status. The status name or description could display when a user hovers
the cursor over the status icon. For instance, a red light in a column
called “Status” could have the tooltip: “X templates failed to process”.
A tooltip can also be useful when a field is disabled due to lack of
prerequisites. If a “Submit” button is disabled because the record is
“Inactive”, then the tooltip can state “Disabled due to being
inactive”.

This feature is available for these controls:

  - Button
  - Combo Box
  - Image
  - List Box

First, write a view with the suffix Dtv for each column that requires a
tooltip, alias the column as “boatooltip” in the view.  

For example, the Finish button on a page is disabled when the Dependency
Complete field is false. To display a short message that says why the
button is disabled, the user creates the following
view.

 

<span style="font-size: 10.5pt;font-family: &#39;Courier New&#39;;color: #1F497D;">CREATE
VIEW
webRequestRoleDtv</span>

<span style="font-size: 10.5pt;font-family: &#39;Courier New&#39;;color: #1F497D;">AS</span>

<span style="font-size: 10.5pt;font-family: &#39;Courier New&#39;;color: #1F497D;">SELECT
RequestID, RoleID, **CASE Validate WHEN 0 THEN 'Dependency not complete
for role' ELSE NULL END AS boaTooltip**</span>

FROM dbo.webRequestRoleDcv

 

The view uses a CASE statement, and sets the column to NULL when the
tooltip should not display.

After the view is written, register it the column.

To register the tooltip view:

1.  <span id="Column Properties Navigation" class="popUpLink">Access the
    *Page Columns* page</span>'s *Vertical* View.

2.  Click **Edit**.
    
    *[View the field descriptions for the Page Columns
    page](../Sys_Admin/Page_Desc/Page_Columns_H.htm)*

3.  Click the **Relational** tab.

4.  Click **Edit**.

5.  Select the view in the **Data Tooltip View** list box.

6.  Enter the binding field name(s) in the **Data Tooltip Binding Field
    Names** text box.
    
    **NOTE:** Include a comma between names.

7.  Click **Save**.
