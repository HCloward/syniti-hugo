+++
title = 'Create a Header Detail Page'
solution = 'Platform'
+++

# Create a Header Detail Page

Header Detail pages, also called Layout pages, are a Page Type that
displays two linked pages in parent and dependent panes.

When creating a Header Detail page:

  - A table is not required.
  - The two pages with views and tables (as in, the parent and child
    page) must be registered to the WebApp but not registered to the
    *Navigation* pane.
  - The two pages must be linked with the Link to Page ID column
    property.
  - The parent page must be assigned to the Parent frame for the Header
    Detail page.
  - The Link To Page ID column must be selected to display in the
    Dependent pane. If multiple columns are linked, it will link to the
    first column by default.
  - The Header Detail page must be added to the *Navigation* pane.

**NOTE:** If the there are multiple buttons on the Header page that link
to different Detail pages, the INITIAL PAGE COLUMN setting must be set
to determine the Detail page that displays when the Header Detail page
opens.

**NOTE:** The INITIAL PAGE COLUMN field must always be completed to
ensure both the Header and Detail pages can automatically open when the
page is being rendered.

To create a Header Detail page:

1.  Select **Admin \> WebApps** on the *Navigation* pane.
2.  Click the **Pages** icon for a WebApp and click **Add**.

OR

1.  Click the WebApp name in the *Navigation* pane.

2.  Click the **Change Settings** icon on the Site toolbar. select
    **Design**, and click **Add.**
    
    [View the field descriptions for the Pages
    page](../Sys_Admin/Page_Desc/Pages_H.htm)

3.  Enter a description of the header page in the **DESCRIPTION** field.

4.  Select **Header Detail** from the **PAGE TYPE** list box.
    
    **NOTE: ** A table is not required for Header Detail Page Types.

5.  Click **Save**, the *Vertical* View displays.

6.  Click **Save**.

7.  Click the **Frames** icon.

8.  Click **Edit** on the row with Priority 10.
    
    [View the field descriptions for the Layout Frames
    page](../Sys_Admin/Page_Desc/Layout%20Frames.htm)

9.  Enter a header page description in the **DESCRIPTION** field.

10. Select the header page ID from the **DEFAULT PAGE ID** list box.
    
    **NOTE:** The **Default Page ID** is the parent page.

11. Click **Save**.

12. Repeat steps 8-11 for the detail page with the priority of 20.

13. Link the pages. Refer to [Link to a Page Using Buttons and
    Images](Link_to_a_Page_Using_Buttons_and_Images.htm) for more
    information.

Continue by [assigning column properties](Assign_Column_Properties.htm).
