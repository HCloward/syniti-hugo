+++
title = 'Re-start a Running Interface'
solution = 'Platform'
+++

# Re-start a Running Interface

With interfaces that have several events, it is common for the events to
take several hours to run. It is possible for an event somewhere in the
process to fail, requiring the interface to be restarted. Advanced users
(who thoroughly understand the interface and its events) can re-start
the interface from the failed event instead of re-starting the interface
from the first event.

**NOTE:** The following process only works if there are no parameters
being passed to the event that failed or any of the subsequent events.
The user must also understand the interface event well enough to know
whether the events that did succeed would need to be re-run for some
reason. On the chance that the interface job might fail, validations can
be added to each event to determine whether or not they need to run.

To re-start an interface at a specific event in Automate:

1.  Disable the events before the event that failed by unchecking
    **Active**. Refer to [Activate Interfaces, Events and
    Validations](Activate_Interfaces_Events.htm) for more information.
2.  Submit the interface again. Refer to [Manually Run an
    Interface](Schedule_Interfaces.htm#Manually) for more information.

## Stop a Running Interface

There are times when it may be necessary to stop a running interface,
such as when a mistake has been discovered or if the interface is taking
an unexpectedly long time to run.

To stop a running interface in Automate:

1.  Click **Monitor** in the *Navigation* pane.
2.  Click **Vertical View** for the interface that needs to be stopped.
3.  Click the **Stop** icon.
