+++
title = 'Create a Dynamic Page'
solution = 'Platform'
+++

# Create a Dynamic Page

The most commonly used page type, a Dynamic page requires a view and an
underlying table. It renders on the fly using the configured settings in
the administrative interface.

A Dynamic page:

  - Displays appropriate data using the Horizontal and Vertical Views in
    the database.
  - Enables proper controls for adding, editing, and deleting records.
  - Sorts the page data as configured.
  - Determines ability to add, edit, delete or sort records on a page.
  - Displays permitted links and appropriate attributes per column as
    designed.

To create a Dynamic page:

1.  Select **Admin \> WebApps** on the *Navigation* pane.
2.  Click the **Pages** icon for a WebApp and click **Add**.

OR

Click the WebApp name in the *Navigation* pane.

Click the **Change Settings** icon on the Site toolbar, select
**Design**, and click **Add**.

[View the field descriptions for the Pages
page](../Sys_Admin/Page_Desc/Pages_H)

Enter a page description in the **DESCRIPTION** field.

Verify **Dynamic** is selected in the **PAGE TYPE** list box.

Select the page’s underlying table from the **TABLE** list box.

Click **Save**; the *Vertical* View displays.

Select the view for the page created in SQL server from the **Horizontal
View** or **Vertical View** list box.

**NOTE:** All dynamic pages must have a table and at least one view.
These list boxes are filtered based on the settings on the Naming
Conventions tab on the *Vertical* View of the
*[WebApps](../Sys_Admin/Page_Desc/WebApps_H)* page. Refer to [Naming
Conventions and the Enforce Strict Naming
Feature](Naming_Conventions_and_the_Enforce_Strict_Naming_Feature)
for more information.

Select a menu from the **Horizontal Menu ID** list box, if using a menu
other than the default.

**NOTE:** The Horizontal menu displays to the left of the page when the
page is accessed. The standard menu is {component name} : Switchboard.

Select an option in the **Insert Method** list box.

**NOTE:** This setting determines the behavior when adding a new record.
Options are:

  - **Not Supported** — No records can be added to the page. The Add
    icon on the Page toolbar does not display.
  - **Horizontal Insert** — Once a record is added and saved, the
    current *Horizontal* View persists.
  - **Horizontal Insert/Switch to Vertical** — Once the record is added
    and saved, the *Vertical* View displays. The *Vertical* View must be
    saved to save any information on the *Vertical* View only. If the
    *Vertical* View is not saved, the data entered on the *Horizontal*
    View persists and still displays.
  - **Horizontal/Switch to Vertical** — Once the record is added and
    saved, the *Vertical* View displays. The *Vertical* View must be
    saved to save any information on the *Horizontal* and *Vertical*
    Views. If the *Vertical* View is not saved, the data entered on the
    *Horizontal* View is not saved.
  - **Switch to Vertical Immediately** — Upon adding a record, the
    *Vertical* View displays.

Select an option from the **Update Method** list box.

**NOTE:** This setting determines the behavior when editing a record.
Options are:

  - **Not Supported** — No records can be edited. The Edit icon on the
    Page Toolbar does not display.
  - **Horizontal Update** — Once a record is edited and saved, the
    current *Horizontal* View persists.
  - **Horizontal Update/Switch to Vertical** — Once the record is edited
    and saved, the *Vertical* View displays. The *Vertical* View must be
    saved to save any information on the *Vertical* View only. If the
    *Vertical* View is not saved, the data edited on the *Horizontal*
    View persists and still displays.
  - **Horizontal/Switch to Vertical** — Once the record is edited and
    saved, the *Vertical* View displays. The *Vertical* View must be
    saved to save any information on the *Horizontal* and *Vertical*
    Views. If the *Vertical* View is not saved, the data edited on the
    *Horizontal* View is not saved.
  - **Switch to Vertical Immediately** — Upon editing a record, the
    *Vertical* View displays.

Click the **Support Delete** check box to disable it, if needed.

**NOTE:** This setting determines if records on the page can be deleted.
When unchecked, the Delete icon does not display on the page.

Click **Save**.

Continue by [assigning page properties](Assign_Page_Properties) or
[assigning column properties](Assign_Column_Properties).
