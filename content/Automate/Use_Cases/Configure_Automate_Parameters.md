# Configure Automate Parameters

The *[Parameters](../Page_Desc/Parameters.htm)* page controls
configuration settings unique per installation. These parameters affect
all interfaces on the site and should only be modified by a developer or
a system administrator.

To configure parameters in Automate:

1.  Select **Configuration \> Parameters** in the *Navigation* pane.

2.  Click **Edit**.
    
    [View the field description for the Parameters
    page](../Page_Desc/Parameters.htm)

3.  Select an administrative role from the **Admin Role** list box.
    
    **NOTE: ** The email addressed configured to the user assigned to
    the Admin Role is used as the From address for the interface
    notification emails. 

4.  Enter a number in the **History Retention Days** field to indicate
    the number of days the interface instance information is
    saved/displayed on the *[Interface
    History](../Page_Desc/Interface_History.htm)* page.
    
    **NOTE:** The history and details about how interfaces were
    processed can be accessed by clicking **History** in the
    *Navigation* pane. By default, history is retained for 30 days.

5.  Select a registered instance from the **Instance** list box.
    
    **NOTE:** The Instance selected MUST match the Instance field in 2
    additional places for email notifications to properly work: *[Role
    (Instance)](../Page_Desc/Role_Instance.htm)* page in Automate and
    the
    *[Parameters](../../Sys_Admin/Page_Desc/Parameters_All_TabsSysAdmin.htm)*
    page in System Administration. Refer to [Set Up Notifications for an
    Interface](Set_Up_Notifications_for_an_Interface.htm) for more
    information.

6.  Be aware of the Filter Info fields (Workflow Filter, Store Procedure
    Filter and Validation Filter). The filters defined are used when
    selecting workflow, stored procedure and validation views within
    Automate. 
    
    **NOTE:** The DSP is delivered with a BOA pre-defined naming
    convention for stored procedures, workflows and validations. The DSP
    uses these naming conventions for populating list boxes in the DSP.
    Do not update these filters; otherwise, list boxes will not populate
    correctly. Refer to [Naming Conventions and the Enforce Strict
    Naming
    Feature](../../WebApp_Dev/Naming_Conventions_and_the_Enforce_Strict_Naming_Feature.htm)
    for more information.  

7.  Select the lowest level of logging Severity that will be written to
    the Log from the **Storage Level** list box. For example, with a
    Storage Level set to “40-Info,” all logging severities 40 and above
    are written to the log.

8.  Select a severity level from the **Reporting By Importance Level**
    list box to determine what severity level icon displays on the
    IMPORTANT field for every record on the
    *[Log](../Page_Desc/Log.htm)* page.

9.  Click the **Log Tasks** check box to enable it, which stores start
    and finish tasks for running events, the interface, etc. in the
    interface’s log.
    
    **NOTE:** To view the log tasks, select Interfaces \> History \> All
    in the *Navigation* pane. If Log Tasks is checked, interface start
    and finish tasks are recorded in the log. Refer to [Add Logging
    Modules](Add_Logging_Modules.htm) for more information.

10. Click **Save**.
