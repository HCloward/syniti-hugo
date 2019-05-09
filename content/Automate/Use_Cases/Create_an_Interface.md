+++
title = 'Create an Interface'
solution = 'Platform'
+++

# Create an Interface

An interface can be created using events, stored procedures, workflows,
etc. to manage a complete business process. The interface can then be
scheduled to run automatically during off hours. 

For example, Automate can connect various corporate systems with SAP and
allow data to flow smoothly between them based on exact specifications.
An Interface Designer can rapidly deploy new interfaces or can modify
existing interfaces without weeks of design and programming.

To create an interface in Automate:

1.  Select **Interfaces** in the *Navigation* pane.

2.  Click **Add**.
    
    [View the field description for the Interfaces
    page](../Page_Desc/Interfaces)

3.  Enter a name of the interface group in the **GROUP** field.

4.  Enter a numeric value in the **ORDER** field to determine the
    interface’s order within the GROUP.
    
    **NOTE:** The GROUP and ORDER fields are used for grouping
    interfaces. Add a record with an identical GROUP name and a
    different ORDER number to configure when interfaces are processed.

5.  Enter a name in the **INTERFACE** field.

6.  Select an ID from the **DATA SOURCE ID** list box.
    
    **NOTE**: The Data Source ID reflects the current list of Data
    Sources registered in the DSP. Select the data source that stores
    the stored procedures, validation views and workflow views used by
    the interface events.

7.  Select an ID from **QUEUE ID** list box. The Queue ID determines
    which service queue is used when the interface runs. This field is
    used to serialize certain operations or for load balance. Options
    are:
    
      - **Background Event–** The background service controls the job
        queue
    
      - **General –** The job is on the General queue
    
      - **Index –** The job is on the Index queue
    
      - **Service Pages–** The associated Service page controls the job
        queue.
        
        **NOTE:** The list of Queue IDs are configured in System
        Administration. Refer to [Add a Service
        Queue](../../Sys_Admin/Use_Cases/Add%20a%20Service%20Queue)
        in the help for more information.

8.  Select a type from **SCHEDULE TYPE** list box to determine when the
    scheduled interface runs. Options are:
    
      - **Frequency–** A numeric value describing how often the schedule
        runs.
    
      - **RunTime –** The specific time when the interface runs.

9.  Enter a time in the **RUN TIME** field.
    
    **NOTE:** The Run Time field must only be populated if the SCHEDULE
    TYPE is set to Run Time. Refer to [Schedule
    Interfaces](Schedule_Interfaces) for more information.
    
    **NOTE:** Ignore THREAD SAFE; this field is not used.

10. Click **Save**; the *Vertical* View displays.
    
    [View the field description for the Interfaces page’s Vertical
    View](../Page_Desc/Interfaces#InterfacesV)

11. Enter a brief description of the interface’s functionality in the
    **Comment** field.

12. Click **Save**.
