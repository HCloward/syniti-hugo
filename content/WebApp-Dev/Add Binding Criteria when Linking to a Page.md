+++
title = 'Add Binding Criteria when Linking to a Page'
solution = 'Platform'
+++

# Add Binding Criteria when Linking to a Page

The Link to Page ID column property allows the page Designer to set the
page that opens when a user clicks a control, such as a button.

By default, when linking from one page to another, the DSP® links the
pages using the key field(s).

However, if the key field(s) are different between linked pages,
identity the key field(s) using Binding Field names. For instance, a
user clicks a button on a *Country* page listing country records to
access a *Region* page listing the selected country’s regions. If the
Country field (the key field) does not have the same name on both pages,
the field on the linked from page (the *Country* page) must be included
as part of the binding criteria. Otherwise, the *Region* page displays
regions for all countries.

If additional fields besides the key fields are required to display
correct data on the linked to page, use Shared Fields to send the data
from a column that is not normally passed and allow the data to be used
on a subsequent page. For example, to filter a Region list box on the
*Region* page by the Country field that was entered on the *Country*
page, add the Country field as a Shared Field on the link between pages.
It is then available for use in the list box Where Clause on the
*Region* page.

In this case, if the Country field is set as a Shared Field and not a
Binding Field, the linked to page (the *Region* page) displays regions
for all countries, but any list boxes with a Country filter display
regions filtered by the country shared from the *Country* page.

To add binding criteria:

1.  <span id="Column Properties Navigation" class="popUpLink">Access the
    Page Columns page.</span>

2.  Click the link in the **LINK TO PAGE** column for the button,
    toolbar button or other control the user clicks to access the linked
    to page.

3.  Click **Edit**.
    
    *[View the field descriptions for the Page Column Links
    page](../Sys_Admin/Page_Desc/Page%20Column%20Links.htm)*

4.  Enter the name of the key field(s) to bind the data from the current
    page to the linked to page in the **Binding Field Names** field.
    
    **NOTE:** Enter multiple columns separated by a comma.

5.  Enter additional field name(s) for columns that are not key fields
    and are not normally passed in the **Shared Field Names** field.
    
    **NOTE:** Enter multiple columns separated by a comma.

6.  Click **Save**.
