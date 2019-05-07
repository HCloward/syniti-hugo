+++
title = 'Configure Data Download During the Final Finish Process to use a DBMoto Package'
solution = 'Master Data Management'
+++

# Configure Data Download During the Final Finish Process to use a DBMoto Package

A process Designer can use DBMoto® for change data capture to replace
final finish package logic. Change data capture is the preferred method
of keeping dspConduct™ in sync with target system(s).

If the Finish Type is DBMoto, then a corresponding Table definition must
exist in Collect. Refer to
[Tables](../../../Platform/Collect/Use_Cases/Register_and_Use_Tables.htm)
in Collect for more information.

This configuration is for documentation purposes only. dspConduct™ does
not start or run the downloads. When configured correctly in Collect,
the DBMoto® synchronization happens automatically.

**NOTE**: dspConduct™ does not confirm that the table exists when
registering a table on the *[Task Final Finish
Tables](../Page_Desc/Task_Final_Finish_Tables_H.htm)* page. An error
displays during the Final Finish if the table does not exist.

**NOTE**: Refer to [Final Finish Process for a Request
Overview](Final_Finish_Process_for_a_Request_Overview.htm) and [Final
Finish Setup Example](Final_Finish_Setup_Example.htm) for general
information.

To register a DBMoto package to download a table for the Final Finish
process:

1.  Click **dspConduct \>Design** in the *Navigation* pane.

2.  Click the **Tasks** icon for a category.

3.  Click the **Final Finish Tables** icon for a parent task (i.e.,
    Request (Address – General), as opposed to Request (Address –
    Telephone/Mobile)).
    
    **NOTE:** Best practice is not to register tables to a child task.

4.  Click **Add**.
    
    [ ](../Page_Desc/Task_Final_Finish_Tables_H.htm)[View the field
    descriptions for the Task Final Finish Tables
    page](../Page_Desc/Task_Final_Finish_Tables_H.htm)

5.  Select **DBMoto** from the **FINISH TYPE** list box.

6.  Enter a number in the **PRIORITY** field.

7.  Click **Save**; *Vertical* View displays.

8.  Select a Collect source from the **Source** list box.

9.  Select a Collect target from the **Target** list box.

10. Select the name of the table to download from the **Table Name**
    list box.

11. Click **Save**.
