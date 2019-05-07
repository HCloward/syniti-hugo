+++
title = 'Configure Data Download During the Final Finish Process to use a CranPort Package'
solution = 'Master Data Management'
+++

 

# Configure Data Download During the Final Finish Process to use a CranPort Package

If the Finish Type is CranPort, then a corresponding Table definition
must exist in Collect. Refer to
[Tables](../../../Platform/Collect/Use_Cases/Register_and_Use_Tables.htm)
in Collect for more information.

<span style="font-weight: bold;">NOTE:</span> dspConduct™ does not
confirm that the table exists when registering a table on the
<span style="font-style: italic;">[Task Final Finish
Tables](../Page_Desc/Task_Final_Finish_Tables_H.htm)</span> page. An
error displays during the Final Finish if the table does not exist.

<span style="font-weight: bold;">NOTE:</span> Refer to [Final Finish
Process for a Request
Overview](Final_Finish_Process_for_a_Request_Overview.htm) and [Final
Finish Setup Example](Final_Finish_Setup_Example.htm) for general
information.

To register a CranPort package to download a table for the Final Finish
process in dspConduct:

1.  Click **dspConduct \> Design** in the *Navigation* pane.

2.  Click the **Tasks** icon for a category.

3.  Click the **Final Finish Tables** icon for a main parent task (for
    example, Request (Address – General), as opposed to Request (Address
    – Telephone/Mobile)).
    
    **NOTE:** It is recommended that tables should not be registered to
    a child task.

4.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Task Final Finish Tables
    page](../Page_Desc/Task_Final_Finish_Tables_H.htm)

5.  Select <span style="font-weight: bold;">CranPort</span> from the
    <span style="font-weight: bold;">FINISH TYPE</span> list box.

6.  Enter a number in the
    <span style="font-weight: bold;">PRIORITY</span> field.
    
    **NOTE:**The execution order of packages is by priority of the role
    (specified on the
    <span style="font-style: italic;">[Role](../Page_Desc/Role_H_dspConduct.htm)</span>
    page) to which the task is assigned, and then the order is specified
    by the order in which the package is added on the
    <span style="font-style: italic;">[Task Final Finish
    Tables](../Page_Desc/Task_Final_Finish_Tables_H.htm)</span> page.

7.  Click **Save**; <span style="font-style: italic;">Vertical</span>
    View displays.

8.  Select a Collect source from the **Source** list box.

9.  Select a Collect target from the **Target** list box.

10. Select the name of the table to download from the **Table Name**
    list box.

11. Select an option in the **Run Rules After Download** list box, if
    applicable.
    
    **NOTE:** This option determines the Collect rules to run on a table
    after download, when a user with the Post role clicks Finish for the
    request on the *[Request Role](../Page_Desc/Request_Role_H.htm)*
    page. Options are:
    
      - **All – Run all of the rules:**  If multiple rules are
        registered to the table in Collect, dspConduct runs them on the
        table after download in the order the rules were added on the
        *[Table
        (Rule)](../../../Platform/Collect/Page_Desc/Table_Rule_H.htm)*
        page in Collect.
    
      - **None – Do not run any rules:** Though rules are registered to
        the table in Collect, dspConduct does not run those rules on the
        downloaded table.
    
      - **NoParametersOnly –** Run only Collect rules that do not
        contain input parameters, such as an Insert rule.
    
      - **ParametersOnly –** Run Collect rules that contain input
        parameters, such as an Update rule.
        
        **NOTE:** The rule(s) must have already been registered and
        activated in Collect.

12. Click **Save**.
