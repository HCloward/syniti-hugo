+++
title = 'Set Up a Category from IGC™ in dspConduct™'
solution = 'Master Data Management'
+++

# Set Up a Category from IGC™ in dspConduct™

When a category is created in IGC™ and imported, a Process Designer must
assign a WebApp to the category and set the category’s owner.

**NOTE**: Each WebApp has one category, so a WebApp must be designed for
each new category created in IGC™.

**NOTE**: When importing a category from IGC™, if there is a category in
dspConduct™ that has the same name, the IGC™ category is automatically
mapped to the dspConduct™ category. If more than one dspConduct™
category has the same name in the database, the IGC™ category is mapped
to the category with the earliest Added On date. All business processes,
scenarios and roles coming from the IGC™ are created as new elements in
the matched category. A process Designer can then map dspConduct™ tasks
to the IGC™ tasks.

To set up the category:

1.  Click **dspConduct \> Design** in the *Navigation* pane.
    
    **NOTE:** If the WEB APP STATUS icon is red, the category must be
    configured.

2.  Click **Edit**.
    
    [View the field descriptions for the Category
    page](../Page_Desc/Category_H.htm)

3.  Select the WebApp name in the **DEFAULT WEB APP ID** list box.
    
    **NOTE**: If the required WebApp does not display in the list box,
    it must be added. In System Administration, refer to [DSP®
    Application
    Development](../../../Platform/WebApp_Dev/Overview_of_DSP_Application_Development.htm)
    for more information about [adding a
    WebApp](../../../Platform/WebApp_Dev/Create_a_WebApp.htm) and to
    [Register a Data
    Source](../../../Platform/Sys_Admin/Use_Cases/Register_a_Data_Source.htm)
    for additional information.

4.  Click **Save**.

5.  Click **Vertical View**.

6.  Click **Edit**.

7.  Select the category owner in the **Owner** list box.

8.  Click **Save**.

Continue with [Map a dspConduct™ Task to a Task Imported from
IGC™](Map_a_dspConduct_Task_to_a_Task_Imported_from_IGC.htm).
