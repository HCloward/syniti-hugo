+++
title = 'Configure Data Download During the Final Finish Process to use a Data Services Job'
solution = 'Master Data Management'
+++

# Configure Data Download During the Final Finish Process to use a Data Services Job

If the Finish Type is DataServices, the Data Services Job must exist in
the repository and the repository must exist as a data source registered
in the platform. Refer to [Register a Data Source in
Common](../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common)
for more information.

<span style="font-weight: bold;">NOTE</span>: Refer to [Final Finish
Process for a Request
Overview](Final_Finish_Process_for_a_Request_Overview) for general
information.

<span style="font-weight: bold;">NOTE</span>: dspConduct™ does not
confirm that the job exists when registering a job or table on the
<span style="font-style: italic;">[Task Final Finish
Tables](../Page_Desc/Task_Final_Finish_Tables_H)</span> page. An
error displays during the Final Finish if the tables or job does not
exist.

To register a Data Services Job to download a table for the Final Finish
process:

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the *Navigation* pane.

2.  Click the **Tasks** icon for a category.

3.  Click the **Final Finish Tables** icon for a main parent task.

4.  It is recommended that tables or jobs should not be registered to a
    child task.

5.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Task Final Finish Tables
    page](../Page_Desc/Task_Final_Finish_Tables_H)

6.  Select **DataServices** from the **FINISH TYPE** list box.

7.  Enter a number in the **PRIORITY** field.
    
    **NOTE:**The execution order of packages is by priority of the role
    (specified on the
    <span style="font-style: italic;">[Role](../Page_Desc/Role_H_dspConduct)</span>
    page) to which the task is assigned, and then the order is specified
    by the order in which the package is added on the
    <span style="font-style: italic;">[Task Final Finish
    Tables](../Page_Desc/Task_Final_Finish_Tables_H)</span> page.

8.  Click **Save**; *Vertical* View displays.
    
    **NOTE:** A Data Services Job might be written to handle a specific
    table. If so, choose the Table Name in the TABLE NAME list box to
    aid in identifying the purpose of that job.

9.  Select the repository that stores the job in the **Data Services
    Data Source** list box.
    
    **NOTE:** The data services repository must be registered as a data
    source.

10. Select the Job name in the **Data Services Job Name** list box.

11. Click **Save**.

To configure Global Variables for a Data Services job::

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Tasks</span> icon for a
    category.

3.  Click the <span style="font-weight: bold;">Final Finish
    Tables</span> icon for a main parent task.

4.  Click <span style="font-weight: bold;">Vertical View</span> for a
    record with the Finish Type of DataServices.

5.  Click the <span style="font-weight: bold;">Global Variables</span>
    icon.

6.  If no records exist, the page displays in add mode. Otherwise, click
    <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Data Services Global Variables
    Setup
    page](../Page_Desc/Data_Services_Global_Variables_Setup_in_dspConduct)

7.  Enter the name of the variable in the
    <span style="font-weight: bold;">NAME</span> field.

8.  Enter the variable value in the
    <span style="font-weight: bold;">CONSTANT</span> field.

9.  Click <span style="font-weight: bold;">Save</span>.
