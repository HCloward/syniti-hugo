+++
title = 'Create a Process'
solution = 'Platform'
+++

# Create a Process

A process, a series of posting steps:

  - Defines how Integrate takes data from the platform and transfers it
    to SAP

  - Serves to link the data in a column in a view with a field on a
    template assigned to the process

Each posting step is a template that is added to the process.

Processes are grouped into categories for organizational purposes.

A process can have multiple templates, but must have at least one
template assigned. Each template is tied to one, or multiple, views.

When a template is added to a process, Integrate imports the loops and
settings from the template into the process.

Once a template has been added to a process, template fields are mapped
to columns in views. Depending on the template type, Integrate may
perform field mapping automatically. A user can also map fields manually
or use the Auto Generate Database Objects feature.

When creating a process, select a template to be assigned to the
process.  After saving the process, add additional templates. Refer to
[*<span style="color: #0000ff;font-style: normal;">Add Templates to a
Process</span>*](Add_Templates_to_a_Process.htm) for more information.

**NOTE**: A user cannot create a process until at least one category and
one active template exist in Integrate because a process is assigned to
a category. A category must have at least one active template before a
process can be created.

A process can be copied to another category. Refer to [Copy a
Process](Copy_a_Process.htm) for more information.

To create a process:

1.  Select **Categories** from *Navigation pane*.

2.  Click the **Processes** icon for a category.
    
    **NOTE:** The number on the **Processes** icon represents the number
    of active and inactive processes assigned to the category.

3.  Click **Add** on Page toolbar; the *Vertical* View displays.
    
    *[View the field descriptions for the Process page’s Vertical
    View.](../Page_Desc/Process_H.htm#Process_V_All_Tabs)*
    
    **NOTE:** At least one active template must exist for the category
    before a process can be added.

4.  Enter a sort value in **Priority**.
    
    **NOTE:** This value determines the order the process displays on
    the *Process* page.

5.  Enter a process name in **Name**.
    
    **NOTE:** A process name must be unique. The process name can
    contain A-Z, 0-9, and underscore. No special characters are allowed
    in process names. Integrate will replace special characters with
    underscores when the process is saved.

6.  Enter a description in **Description**.

7.  Select a template from **Template ID** list box.
    
    **NOTE:** The **Template ID** list box only displays active
    templates assigned to the category.

8.  Select a data source from **Data Source ID** list box.
    
    **NOTE:** The **Data Source ID** list box displays all data sources
    registered to the platform’s instance.

9.  Select an option in the **View Name** list box.
    
    **NOTE:** If a view is selected for this template type, the view
    will be assigned to all process template loops. The recommended
    practice is to select a View Name if a process is based on a
    template with only one loop.
    
    **NOTE:** If the process will use the Auto Generate Database Objects
    feature, or if the process will be based on multiple templates with
    difference views, do not select an option in the **View Name** list
    box.

10. Click **Save**; the **Template ID** is automatically registered to
    the process.
    
    **NOTE:** After the process is saved, the **View Name** field no
    longer displays on the *Vertical* View.

11. Click **Documentation** tab.

12. Click **AdvancedProperties** tab.

13. Select the **Synchronous** posting method from **Post Execution
    Method** list box if the process will have multiple templates
    assigned and will use transaction stringing.
    
    **NOTE:** A process that uses the **Asynchronous** post execution
    method, the option that is selected by default, executes the post
    for each template sequentially without waiting for the template post
    to return before executing the next template post. Asynchronous
    posting may result in locking, especially when posting a combination
    of GUI and BDC templates in the same process. A process that uses
    the **Synchronous** post execution method executes the post for each
    template but waits for the post to return before executing the next
    post. Synchronous is a slower execution method but prevents most
    recording locking situations.

14. Enter a value (in milliseconds) in **Delay Between Templates** if
    the process will have multiple templates assigned.
    
    **NOTE:** The default value is 0 seconds, which indicates there is
    no delay between the execution of templates during a post. Enter a
    value greater than 0 if posting a multiple template process that
    contains transactions that take some non-trivial time to save and
    exit. This situation is more common when working with GUI Script
    templates than with BDC Script templates.

15. Enter a value (in milliseconds) in the
    <span style="font-weight: bold;">Delay Between Records</span> field
    to set the amount of time that passes after processing of one record
    is complete and processing of the next record can begin.
    
    **NOTE:** Unless the value is entered here, there is no delay
    between record processing, which could result in data locking
    issues.

16. Click **Save**.

17. Add additional templates, if applicable.

**NOTE:** Refer to [Add Templates to a
Process](Add_Templates_to_a_Process.htm) for detailed information.
