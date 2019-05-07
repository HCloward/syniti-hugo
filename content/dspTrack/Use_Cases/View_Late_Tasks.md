+++
title = 'View Late Tasks'
solution = 'Platform'
+++

# View Late Tasks

A task is late if the task is not in a Completed status and:

  - The current date is later than the planned finish date or
  - The task is on the critical path and a task that occurs before it in
    the critical path is late or
  - The task has passed a Threshold Warning. Refer to [Set Parameters
    for Task Status
    Calculation](Set_Parameters_for_Schedule_Status_Calculation.htm) for
    more information about Threshold Warnings.

When a task is late, it displays on the *Late Task* page. Late tasks
only display for active plans. If a plan is deactivated, the late tasks
associated with that plan when the plan was active no longer display on
the *Late Task* page.

Work List items added on the *Work List Setup* page that are late do not
appear as late tasks.

<span style="font-weight: bold;">NOTE</span>: Security settings are
required to view late tasks on the *<span>Late Task</span>* page. To
view late tasks, users must be assigned to the Sample Project Level Role
or the Sample Plan Level Role. If custom security roles are defined,
these roles must have at least one of the following WebApp Groups
assigned: Power User, Power Designer, Project User or Plan User to view
late tasks.

**NOTE**: Security keys must be assigned to a security role every time a
new project or plan is created in dspTrack™.

Refer to [Set Up Security for
dspTrack™](../Config/Set_Security_in_dspTrack.htm) for more
information.

There are two ways to access the *Late Task* page: view all late tasks
across all projects or view late tasks for a plan.

To view all late tasks across all projects, select **Late Tasks** in the
*Navigation* pane.

To view late tasks for a plan:

1.  Click <span style="font-weight: bold;">Project </span>in the
    *Navigation* pane.
2.  Click **Plans** for a project.
3.  Click **Vertical View** for a plan.
4.  Click the **Additional Information** tab.
5.  Click **Late Tasks**.

**NOTE**: The Late Tasks icon will always display red, even if there are
no late tasks associated with the plan.
