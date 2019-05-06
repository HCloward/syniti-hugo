# Receive Workflow Messages

dspTrack™ sends workflow messages to users assigned to a Plan Task or
Work List Item under certain conditions. Settings can configure how
users receive the workflow messages, and how long these messages are
retained.

Users can receive messages as an email, a message displayed in the DSP®,
or both. Refer to [Set User Workflow Receipt
Preferences](Set_User_Workflow_Receipt_Preferences.htm) for more
information.

dspTrack™ sends workflow messages to users assigned to a Plan Task or
Work List Item when:

  - **Work on that task or item has started.** A user starts work by
    clicking Next Action for the item or task on the Work List. All
    other users assigned to the item will receive one message. The user
    who started the work will not receive a message. Refer to [Task
    Status](../Page_Desc/Task_Status1.htm) for more information about
    how tasks and items move through the workflow.

  - **A Plan Task is ready to be worked on because all of its
    predecessor tasks are complete.** Each assigned user will receive
    one message when a user clicks Next Action on the Work List to
    complete the final required predecessor task.
    
    **NOTE:** Work List Items do not have predecessor tasks.

  - **The current date is later than the planned start date for an item
    or task**. dspTrack™ sends a message once per day per user for any
    late task or item. The message is sent every day the task or item is
    late, and includes the number of days that have passed since the
    planned start date. Once a user clicks Next Action on the Work List
    to start work on the task or item, no more wor flow messages are
    sent.

  - <span>**A task is late or in danger of being late according to
    schedule status calculations.** Refer to [Set Parameters for
    Schedule Status
    Calculations](Set_Parameters_for_Schedule_Status_Calculation.htm)
    for more information.</span>

<span style="font-weight: bold;">NOTE</span>**:** Work List Items are
not affected by schedule status calculations.

**NOTE**: On the *Parameters* page, on the Workflow tab, the Workflow
Retention Days setting determines the number of days workflow messages
are retained before they are deleted.

Workflow messages that have been sent display on the
*<span style="font-size: 10.0pt;">Log</span>* page. Refer to [View
Workflow Messages Sent](View_Workflow_Messages_Sent.htm) for more
information.
