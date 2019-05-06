# Schedule Interfaces

By default, an interface runs on a schedule with a run time of 12:00
A.M. daily, but it can be altered to run at any time of day, down to the
second.

If an interface does not have a schedule (as in., the Schedule Info
fields are not populated on the *Vertical* View of the
*[Interfaces](../Page_Desc/Interfaces.htm#InterfacesV)* page), the
interface must be run manually until a schedule is added.

**NOTE:** It is recommended to synchronize Retry Intervals and Interface
Schedules so that two instances of the same interface are not attempting
to run at the same time.  Refer to [Set Retry
Parameters](Set_Retry_Parameters.htm) for more information.

Interfaces can be scheduled to run two ways (as determined by the
SCHEDULE TYPE field):

  - **Frequency –** A numeric value describing how often the schedule
    runs.
  - **RunTime –** The specific time when the interface is run.

## Run an Interface on a Frequency Schedule

Running an interface on a Frequency schedule allows users to determine
how often an interface runs, for example, every 10 minutes or once a
month. Users cannot, however, configure the exact time of day the
interface runs.

**NOTE:** The exact time the interface runs is determined by how
frequently the [Interface
(Initiator)](Configure_Automate_Service.htm#InterfaceInitiator) service
page runs. By default, this service page runs every 30 seconds (refer to
the [Configure Automate Service Pages](Configure_Automate_Service.htm)
section for information on the recommended schedule).

When the Interface (Initiator) service pages runs, an interface is
submitted to run if:

  - The current date is greater than the last run time of the Automate
    job plus the configured Frequency, and
  - The day that the interface is to run is enabled on the Schedule Info
    tab of the interface

To run an interface on a Frequency schedule in Automate:

1.  Select **Interfaces** in the *Navigation* pane.

2.  Click **Vertical View** for desired interface.

3.  Click the **Schedule Info** tab.

4.  Click **Edit**.
    
    [View the field description for the Interfaces page’s Vertical
    View](../Page_Desc/Interfaces.htm#InterfacesV)

5.  Enter the number of times an interface is run per chosen unit of
    measure in the **Frequency** field.

6.  Select a unit of measure at which the frequency runs from the
    **UOM** list box. Options are Day, Hour, Minute, Month, and Second.

7.  Click the check boxes next to the names of the select day(s) of the
    week the interface is to run.
    
    **NOTE:** The Days field is automatically populated with when the
    interface is schedule to run, based on the information populated in
    the Frequency and UOM fields.

8.  Click **Save**.

**Example:**

**Frequency:** 5 minutes

**Days:** Monday and Wednesday

On Monday at 12:00 A.M., the interface is submitted once the *Interface
(Initiator)* service page runs and the current date is greater than the
last run time of the Automate job plus the Frequency set for the
interface schedule. If it takes the service page 3 minutes to run and
the Frequency is 5 minutes, the interface is submitted at 12:08 A.M. The
interface continues to run on this schedule until Tuesday at 12:00 A.M.
The same schedule begins again on Wednesday at 12:00 A.M and runs until
Thursday at 12:00 A.M.

## Run an Interface on a RunTime Schedule

Running an interface on a Run Time schedule allows users to select a
specific reoccurring date and time to run the interface.

To run an interface on a Run Time schedule in Automate:

1.  Select **Interfaces** in the *Navigation* pane.

2.  Click **Vertical View** for desired interface.

3.  Click the **Schedule** Info tab.

4.  Click **Edit**.
    
    [View the field description for the Interfaces page’s Vertical
    View](../Page_Desc/Interfaces.htm#InterfacesV)

5.  Enter the specific time when the interface is to run in the **Run
    Time** field.

6.  Click the check boxes next to the names of the select day(s) of the
    week the interface is to run.
    
    **NOTE:** The Days field is automatically populated with when the
    interface is schedule to run, based on the information populated in
    the Run Time and Day Info fields.

7.  Click **Save**.

## <span id="Manually"></span> Manually Run an Interface

Interfaces can be manually run to test the interface, to rerun the
interface due to errors in the last run, or if the interface needs to be
run before the next scheduled time.

To manually run an interface in Automate:

1.  Select **Interfaces** in the *Navigation* pane.
2.  Click **Vertical View** for the interface. Run options are:

<!-- end list -->

  - **Debug –** Immediately runs the interface in the foreground with
    full logging information. Debug Mode must be enabled on the
    *Vertical* View of the
    *[Interfaces](../Page_Desc/Interfaces.htm#InterfacesV)* page.

  - **Execute –** Immediately runs the interface in the foreground.

  - **Submit –** Submits the interface to run in the background.

**NOTE:** These icons are only active when ACTIVE is enabled for the
interface.
