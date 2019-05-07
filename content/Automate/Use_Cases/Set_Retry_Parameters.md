+++
title = 'Set Retry Parameters'
solution = 'Platform'
+++

# Set Retry Parameters

The Retry Parameters, in conjunction with Event Validations, allow the
Interface Developer to communicate with Automate that an earlier event
may still be running and that this interface event should wait, allowing
the other event to complete.  Retry Parameters should be set close to
the usual time it takes an event to complete. A running interface will
fail when the maximum Retry Interval has been reached. This mechanism
prevents an interface from running indefinitely. Since simple workflow
events are expected to execute quickly, the Retry Parameters are not
necessary for workflow events.

**NOTE**: It is recommended to synchronize Retry Intervals and Interface
Schedules so that two Instances of the same interface are not attempting
to run at the same time. Refer to [Schedule
Interfaces](Schedule_Interfaces.htm) for more information.

Once you have created an interface and added an event, set the Retry
Parameters.

To set Retry Parameters in Automate:

1.  Select **Interfaces** in the *Navigation* pane.

2.  Click the **Events** icon for the desired interface.

3.  Click **Vertical View** for the event.

4.  Click **Retry Parameters** to expand the section.

5.  Click **Edit**.
    
    [View the field description for the Interface Events page’s Vertical
    View](../Page_Desc/Interface_Events.htm#InterfaceEventsV)

6.  Enter an interval at which to retry running the stored procedure
    event in the **Retry Interval** field.

7.  Enter a maximum retry interval at which to retry running the stored
    procedure event in the **Maximum Retry Interval** field.

8.  Select a unit of measure from the **Retry Interval UOM** list box.
    Options are Day, Hour, Minute, Month or Second.
    
    **NOTE**: If the Retry Interval Field is set 5, and the UOM is set
    to Hours, when the stored procedure fails, the DSP will try to run
    it again in 5 hours. The Max Retry Interval field is the number of
    times that the stored procedure is set to run until it stops. If
    that value is 10, then when the stored procedure fails, it will
    retry every 5 hours for 10 times and then stop.

9.  Click **Save**.
