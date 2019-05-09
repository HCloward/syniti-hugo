+++
title = 'Escalate Late Tasks'
solution = 'Platform'
+++

# Escalate Late Tasks

A user assigned to the DSPTrack.Project.Template or
DSPTrack.Plan.Template security roles can escalate late tasks for a
project.

**NOTE**: The security keys for the project and plan must have been
added to the security role as well. Refer to [Set Up Security for
dspTrack™](../Config/Set_Security_in_dspTrack) for more information.

When viewing all tasks in all projects (select **Late Tasks** in the
*Navigation* pane), the managers that display on the *Late Task
Escalation* page depend on whether work on the late task selected on the
*Late Task* page has begun. Work starts for a task when a user clicks
Next Action on the Work List when a task is in Ready status.

If work on a late task has not begun (the task is in Ready or Waiting on
Dependency status) the *Late Task Escalation* page displays the
escalation managers from all escalation processes associated with
business users assigned to the task selected on the *Late Task* page.

If work on a late task has begun (the status of the task is In Progress)
the *Late Task Escalation* page displays the managers for the business
user who started work on the task. <span> </span>

<span style="font-weight: bold;">NOTE</span>: The order that a contact
displays on the <span style="font-style: italic;">Late Task
Escalation</span> page is determined by the priority set for a contact
on the <span style="font-style: italic;">User List – Receive Workflow
Escalation</span> page (Configuration \> Workflow \> Escalation
Process).

To escalate a late task:

1.  Select **Late Tasks** in the *Navigation* pane to view all late
    tasks across all projects.
    
    OR.
    
    Select **Project \> Plans \> Vertical View \> Additional Information
    tab \> Late Tasks** to view late tasks for a plan.

2.  Select the task that requires the escalation email to be sent.
    
    **NOTE**: If no records display on the *Late Task Escalation* page,
    an Escalation process has not been created for users assigned to
    that task.

3.  Click **Send Escalation Email** for the contact NAME on the *Late
    Task Escalation* page.

The ESCALATED ON field updates to the date and time the email was sent.

The ESCALATED BY field updates with the user name of the user who
clicked Send Escalation Email.
