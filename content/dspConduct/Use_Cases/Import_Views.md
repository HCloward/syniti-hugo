# Import Views

This section contains the following topics:

  - [Import a Task View for a
    Category](#Import_a_Task_View_for_a_Category)
  - [Import a Variant View for a
    Category](#Import_a_Variant_View_for_a_Category)

## <span id="Import_a_Task_View_for_a_Category"></span>Import a Task View for a Category

A Designer uses the <span style="font-style: italic;">[Category Import
View
Configuration](../Page_Desc/Category_Import_View_Configuration.htm)</span>
page to import a task view for a category.

Before performing this task, the design process must be complete and a
task must be defined in the Content WebApp. Refer to [dspConduct™ Design
Process Overview](dspConduct_Design_Process_Overview.htm) for more
information.

To import a task view for a category in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \>
    </span>**Configuration \> Configuration Import** in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Select a category.

3.  Click **Edit**.
    
    *[View the field descriptions for the Category Import View
    Configuration
    page.](../Page_Desc/Category_Import_View_Configuration.htm)*

4.  Select a task view to import from the **TASK IMPORT VIEW** list box.

5.  Click **Save**.

6.  Click the **Task Import Required Columns** icon in the Page toolbar
     to see the required columns for the task view.

7.  Click the **Import Tasks** icon.
    
    *[View the field descriptions for the Task Import Staging
    page.](../Page_Desc/Task_Import_Staging.htm)*
    
    **NOTE:** The task records in the view are compared to the task
    records in the WebApp. If the Action field is Change, the task
    exists in the WebApp, and if the task in the view differs from the
    task in the WebApp, the WebApp is updated on import. If the Action
    field is New Task, the task is not in the WebApp.
    
    **NOTE:** Optional fields for task import are comments and
    instructions. If included in the view, they are imported. If
    comments and instructions are different in the view and the WebApp,
    the WebApp is updated.
    
    **NOTE**: Import only adds or updates tasks. Existing tasks in the
    WebApp are not deleted.

8.  To exclude certain tasks from the import, select one or more tasks,
    and then click the **Deactivate** icon to disable the **ACTIVE**
    check box.
    
    **NOTE:** The ACTIVE check box is enabled by default. Tasks for
    which the ACTIVE check box is disabled are not imported.

<!-- end list -->

1.  Click
**Import**.

## <span id="Import_a_Variant_View_for_a_Category"></span>Import a Variant View for a Category

A Designer can import a variant view for a category. A variant view
includes the column settings for the variant.

Before performing this task, the design process must be complete and a
task must be defined in the Content WebApp. Refer to [dspConduct™ Design
Process Overview](dspConduct_Design_Process_Overview.htm) for more
information.

To import a variant view for a category in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \>
    </span>**Configuration \> Configuration Import** in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Select a category.

3.  Click **Edit**.
    
    *[View the field descriptions for the Category Import View
    Configuration
    page.](../Page_Desc/Category_Import_View_Configuration.htm)*

4.  Select a variant view to import from the **VARIANT IMPORT VIEW**
    list box.

5.  Click **Save**.

6.  Click the **Variant Import Required Columns** icon to see the
    required columns for the variant view.

7.  Click the **Import Variants** icon.
    
    *[View the field descriptions for the Variant Import Staging
    page.](../Page_Desc/Variant_Import_Staging.htm)*
    
    **NOTE**: The parent pane displays the variants in the view (the
    conditions for each column). The child pane displays column settings
    (required and control status) for the variants.
    
    **NOTE**: The variant records in the view are compared to the
    variants in the WebApp. If the Action field is Change, and the
    variant exists in the WebApp for the scenario \> role \> task
    combination, the record is updated with the values in the view when
    imported. If the Action field is New Variant the variant is not in
    the WebApp.
    
    **NOTE**: Import only adds or removes variants. Existing variants in
    the WebApp are not deleted.

8.  To exclude certain variants from the import, select one or more
    variants, and then click the **Deactivate** icon to disable the
    **ACTIVE** check box.
    
    **NOTE**: The ACTIVE check box is enabled by default. Variants for
    which the ACTIVE check box is disabled are not imported. Enabling or
    disabling the ACTIVE check box for a variant enables/disables all of
    the associated column settings for the variant.

9.  To view the column settings for a variant, click the **Columns**
    icon.

10. To update a column setting select the record and click **Edit**.
    
    *[View the field descriptions for the Variant Column Import Staging
    page.](../Page_Desc/Variant_Column_Import_Staging.htm)*

11. Select the default value for the column from the **CONTROL STATUS**
    list box.

12. Click the **REQUIRED** check box to enable or disable it as needed.

13. Click **Save**.

14. To exclude certain column settings from the import, select one or
    more column settings, and then click the **Deactivate** icon to
    disable the **ACTIVE** check box.
    
    **NOTE:** The ACTIVE check box is enabled by default. Column
    settings for which the ACTIVE check box is disabled are not
    imported.
    
    **NOTE:** To activate or deactivate all of the column settings for a
    variant, click the <span style="font-weight: bold;">Activate</span>
    or <span style="font-weight: bold;">Deactivate</span> icon on the
    *Variant Import Staging* page (parent page).

15. Repeat Steps 9 – 13 to update the column settings for other variants
    as needed

16. Click **Import**.
