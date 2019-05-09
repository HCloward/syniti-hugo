+++
title = 'Add Column Help Text'
solution = 'Platform'
+++

# Add Column Help Text

A page designer can assign help text to a specific column on a page in a
custom WebApp. This type of help, called Dynamic Help or Page Column
Help, can be added at the WebApp level or the Page level using catalogs.
To view column help, hover over the column heading. The help displays
below the *Navigation* pane in the Information pane. By default the
column name and field name display if column help has not been added.

Refer to [Use Catalogs During Application
Development](../Sys_Admin/Use_Cases/Use_Catalogs) for general
information.

A page designer can also [Add Dynamic Help to a
Page](addDynamicHelpToAPage), which involves the assignment of help
text to a page itself.

Adding Column Help Text requires the completion of three tasks:

1.  [Create a WebApp
    Catalog](../Sys_Admin/Use_Cases/Create_WebApp_Catalogs).

2.  .[Assign a Catalog to a Custom
    WebApp](../Sys_Admin/Use_Cases/Assign%20a%20Catalog%20to%20a%20Custom%20Webapp)

3.  Add Page Column Help Text at the WebApp Level.
    
    OR
    
    Add Page Column Help Text at the Page Level.

## Add Page Column Text at the WebApp Level

For page help text to display for a column wherever it appears in a
custom WebApp, add it to the assigned catalog at the WebApp level.

To add dynamic help to a catalog at the WebApp level:

1.  Select **Admin \> Translations \> Catalogs** in the *Navigation*
    pane.

2.  Click the **Phrases** icon for the catalog you created for this
    help.
    
    **NOTE:** You must create a new catalog to add dynamic help to a
    column. See [Create WebApp
    Catalogs](../Sys_Admin/Use_Cases/Create_WebApp_Catalogs) for
    more information.
    
    **NOTE:** If no record exists, the page displays in add mode.
    Otherwise, click **Add**.
    
    [View the field descriptions for the Catalog Phrases
    page](../Sys_Admin/Page_Desc/Catalog_Phrases)

3.  Enter the technical field name for the column to add dynamic help to
    in the **PHRASE** field.
    
    **NOTE:** For example, KUNNR or Name1. The spacing must be identical
    to how it appears in the table.

4.  Enter the display name of the column to add dynamic help to in the
    **PHRASE OUT** field.
    
    **NOTE:** For example, Customer or Name.

5.  Click **Save**.

6.  Click **Cancel** to exit add mode.

7.  Click **Vertical View** for the Catalog Phrase you just added.

8.  Click **Edit**.

9.  Enter the help text to display for the column in the **DYNAMIC
    HELP** text box.

10. Click **Save**.

## Add Page Column Help Text at the Page Level

For page column help to display for a column only on a specific page in
a custom WebApp, add column help text at the page level.

To add dynamic help to a column at the page level:

1.  Access the WebApp page.

2.  Click the **Change Settings** icon on the Site toolbar.

3.  Select **Design** from the drop down menu.

4.  Click the **Column Properties** icon.

5.  Click the **Help** icon for the column.
    
    **NOTE:** If not in Add mode, click the **Add** button.
    
    [View the field descriptions for the Catalog Phrase Translations
    (Page Specific)
    page](../Sys_Admin/Page_Desc/Catalog%20Phrase%20Translations%20Page%20Specific)

6.  Select the Catalog ID of the catalog that contains the help you want
    to display from the **Catalog ID** list box.

7.  Enter the text that displays as help in the **Dynamic Help** Editor
    field.

8.  Click **Save**.
