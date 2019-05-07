+++
title = 'Register Tables for Download through Data Services'
solution = 'Data Quality'
+++

# Register Tables for Download through Data Services

**NOTE**: The Data Services job must have been written and stored in the
Data Services repository before the job can be registered in
dspCompose™.

Data Services jobs can be registered and run to pull data from the SAP
environment and add it to the dgSAP database (the working snapshot of
the SAP data).

The RequestID, as the global variable "$RequestID", is always passed to
the Data Services job during the dspCompose™ Finish process. RequestID
does not need to be registered.

If additional global variables are needed, they can be added on the
<span style="font-style: italic;">[Data Services Global Variables
Setup](../Page_Desc/Data_Services_Global_Variables_Setup.htm)</span>
page.

**NOTE:** Refer to[Troubleshoot Data Download Using a Data Services
Job](Troubleshoot_Data_Download_Using_a_Data_Services_Job.htm) if the
job does not run as expected or if the job must be run again.

To register a Data Services job:

1.  Select **Team** in the *Navigation* pane.

2.  Click the **Templates** icon for a team.

3.  Click the **Roles** icon for a template.

4.  Click <span>the **Finish Tables** icon</span> for the Post role.
    
    **NOTE:** If no records exist, the page displays in add mode.
    Otherwise, click <span style="font-weight: bold;">Add</span>.
    
    *[View the field descriptions for the Template Role (Finish)
    page](../Page_Desc/Template_Role_Finish.htm)*

5.  Select the name of the Data Services repository that stores the Data
    Services job in the **DATA SERVICES DATA SOURCE** list box.

6.  Select the name of the Data Services job in the **DATA SERVICES JOB
    NAME** list box.

7.  Click **Save**.
