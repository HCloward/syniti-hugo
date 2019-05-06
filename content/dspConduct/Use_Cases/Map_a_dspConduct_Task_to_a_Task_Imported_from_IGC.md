# Map a dspConduct™ Task to a Task Imported from IGC™

After a task has been created and published in IGC™ and imported into
dspConduct™, a Process Designer must map at least one dspConduct™ task
to it.

An IGC™ task can have multiple dspConduct™ tasks assigned.

An IGC™ task can be mapped to:

  - [An existing task in
    dspConduct™](#Map_an_IGC_Task_to_An_Existing_dspConduct_Task),
    including the delivered tasks Request Post and Request Post Workflow
    Notification
  - [A new task based on a page that already exists in the Content
    WebApp](#Map_an_IGC_Task_to_a_New_Task_Based_on_an_Existing_Page_in_the_Content_WebApp)
  - [A new task based on a new page created in the Content
    WebApp](#Map_an_IGC_Task_to_a_New_Task_Based_on_a_New_Page_in_the_Content_WebApp)

**NOTE:** To create a new dspConduct™ task based on a new page in the
Content WebApp, a user must be assigned to the Power Designer and
Designer roles in System Administration and the Administrator role in
the Content WebApp assigned to that category.

Before performing these steps, [Set Up a Category from IGC™ in
dspConduct™](Set_Up_a_Category_from_IGC_in_dspConduct.htm) if needed.

**NOTE:** When a Post role is imported into dspConduct™, if the role has
no IGC™ tasks assigned to it one dspConduct™ generic Post task is
created for the Post role.

After mapping is complete, pages in dspConduct™ update to reflect the
mappings. If existing dspConduct™ task(s) have been mapped to an IGC™
task, the Role Task page(s) and the Scenario Role Task page(s) update to
reflect these mappings. If an IGC™ task is mapped to a new dspConduct™
task, the Task page is updated.

**NOTE:** To view the roles to which the selected IGC™ task is assigned,
click the Roles button on the *[IGC Task](../Page_Desc/IGC_Task.htm)*
page. From there, after a task is assigned to the role, click the Where
Used icon to view the scenarios and business processes that use the role
task.

## <span id="Map_an_IGC_Task_to_An_Existing_dspConduct_Task"></span>Map an IGC™ Task to An Existing dspConduct™ Task

After an IGC™ task is imported into dspConduct™ for the first time, it
must be mapped to an existing dspConduct™ task. If the task is
republished in IGC™ and imported again, the task mapping is not updated.
If the IGC™ task is deleted in IGC™, the mapping is removed, but the
dspConduct™ task is not otherwise affected. If the task is deleted in
the Content WebApp, the IGC™ task must be mapped to another dspConduct™
task.

To map an IGC™ task to an existing dspConduct™ task:

1.  Click **dspConduct \> Design** in the *Navigation* pane.

2.  Click the **IGC Tasks** icon for the category.

3.  Click the **Use Existing Tasks** icon.

4.  Select the name of the dspConduct™ task in the **TASK ID** list box.
    
    **NOTE:** The list box displays tasks of the same task type as the
    IGC™ task selected on the [IGC Task](../Page_Desc/IGC_Task.htm)
    page. If the IGC™ task is a Post type task, the delivered tasks
    Request Post and Request Post Workflow Notification are also
    available.

5.  Click **Save**.

**NOTE:** If an error has occurred in the framework while attempting to
map the IGC™ task to the existing dspConduct™ task an error message
displays and the PUBLISHED field is unchecked. Click the log link in the
error message for more information.

Continue with [Update Custom Attributes for Governance
Elements](Update_Custom_Attributes_for_Governance_Elements.htm), if
needed.

## <span id="Map_an_IGC_Task_to_a_New_Task_Based_on_an_Existing_Page_in_the_Content_WebApp"></span>Map an IGC™ Task to a New Task Based on an Existing Page in the Content WebApp

A page that has been created in the Content WebApp can be mapped to an
imported IGC™ task. If the task is republished in IGC™ and imported
again, the task mapping is not updated. If the IGC™ task is deleted in
IGC™, the mapping is removed, but the dspConduct™ task is not otherwise
affected. If the page is deleted in the Content WebApp, the IGC™ task
must be mapped to another dspConduct™ task.

To map an IGC™ task to a new task based on a page that exists in the
Content WebApp:

1.  Select **dspConduct \> Design** in the *Navigation* pane.

2.  Click the **IGC Tasks** icon for the category.

3.  Click the **Create New Task** icon for the IGC™ task.

4.  Enter a description of the task in the **DESCRIPTION** field, or
    retain the default (the name of the IGC™ task).
    
    **NOTE:** It is recommended to give the task a unique name to
    identify it.

5.  Enter a comment about the task in the **COMMENT** field, if needed.

6.  Enter instructions in the **INSTRUCTIONS** field, if needed.

7.  Click **Save**.

8.  Click the **Use Existing Page** icon.

9.  Click **Edit**.
    
    *[View the field descriptions for the Assign IGC Task to Existing
    Page page](../Page_Desc/Assign_IGC_Task_to_Existing_Page.htm)*

10. Select the page from the **EXISTING PAGE** list box.
    
    **NOTE:** Only pages stored in the WebApp assigned to the category
    display.

11. Click the **RENAME PAGE** check box, if needed.
    
    **NOTE:** If enabled, the page name is updated to the IGC™
    description.

12. Click **Save**.

13. Click the **Link New Task to Existing Page** icon in the Page
    toolbar.

After a task has a page assigned, it displays on the
*[Task](../Page_Desc/Task_H.htm)* page.

Continue with [Update Custom Attributes for Governance
Elements](Update_Custom_Attributes_for_Governance_Elements.htm), if
needed.

## <span id="Map_an_IGC_Task_to_a_New_Task_Based_on_a_New_Page_in_the_Content_WebApp"></span>Map an IGC™ Task to a New Task Based on a New Page in the Content WebApp

**NOTE:** To create a new dspConduct™ task based on a new page in the
Content WebApp, a user must be assigned to the Power Designer and
Designer roles in System Administration and the Administrator role in
the Content WebApp assigned to that category.

To map an IGC™ task to a new task based on a new page in the Content
WebApp:

1.  Click **dspConduct \> Design** in the *Navigation* pane.

2.  Click the **IGC Tasks** icon for the category.

3.  Click the **Create New Task** icon for the IGC™ task.

4.  Enter a description of the task in the **DESCRIPTION** field, or
    retain the default (the name of the IGC™ task).
    
    **NOTE:** It is recommended to give the task a unique name to
    identify it.

5.  Enter a comment about the task in the **COMMENT** field, if needed.

6.  Enter instructions in the **INSTRUCTIONS** field, if needed.

7.  Click **Save**.

8.  Click the **Create Page** icon.
    
    **NOTE:** The
    *[Pages](../../../Platform/Sys_Admin/Page_Desc/Pages_H.htm)* page in
    System Administration displays with the name of the IGC™ task in the
    DESCRIPTION field.

9.  Update the page name in the **DESCRIPTION** field if needed.

10. Select **Dynamic** or **Header Detail** from the **PAGE TYPE** list
    box.
    
    **NOTE:** No other page types are allowed when mapping a page to an
    IGC™ task.

11. Select the table underlying the page in **TABLE** list box.
    
    **NOTE:** Design the page as needed. Refer to [DSP® Application
    Development](../../../Platform/WebApp_Dev/Overview_of_DSP_Application_Development.htm)
    for more information.

12. Click the **Use Existing Page** icon once the page has been saved.

13. Click the **RENAME PAGE** check box, if needed.
    
    **NOTE:** If enabled, the page name is updated to the IGC™
    description.

14. Click **Save**.

15. Click the **Link Cloud Task to Page** icon in the Page toolbar.

After a task has a page assigned, it displays on the
*[Task](../Page_Desc/Task_H.htm)* page.

Continue with [Update Custom Attributes for Governance
Elements](Update_Custom_Attributes_for_Governance_Elements.htm), if
needed.
