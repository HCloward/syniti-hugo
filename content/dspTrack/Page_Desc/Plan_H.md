+++
title = 'Plan H'
solution = 'Platform'
+++

# Plan H

[Plan V](#Plan_V)

<div class="use">

Use this page to [Organize Plans with
Projects](../Use_Cases/Organize_Plans_with_Projects).

</div>

To access this page:

1.  Click **Track \> Project** in *Navigation* pane.
2.  Click **Plans**.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Copy Plan</p></td>
<td><p>Click to open the <em><a href="../Use_Cases/Copy_Plan">Copy Plan</a></em> page to create a new plan based on a copy of the selected plan.</p></td>
</tr>
<tr class="odd">
<td><p>NAME</p></td>
<td><p>Displays the plan name.</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If enabled, the plan has been activated and plan tasks for the plan display on the Work List.</p></td>
</tr>
<tr class="odd">
<td><p>PLANNED START DATE</p></td>
<td><p>Displays the earliest start date of all tasks in the plan according to the project schedule.</p></td>
</tr>
<tr class="even">
<td><p>PLANNED FINISH DATE</p></td>
<td><p>Displays the latest finish date of all tasks in the plan according to the project schedule.</p></td>
</tr>
<tr class="odd">
<td><p>Tasks</p></td>
<td><p>Click to open the <em><a href="Plan_Task_H">Plan Task</a></em> page to add, configure and delete plan tasks from the plan. The number on the icon represents the number of tasks in the plan.</p>
<p>Refer to <a href="../Use_Cases/Work_with_Plan_Tasks">Work With Plan Tasks</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Tags</p></td>
<td><p>Click to open the <em><a href="Plan_Tag"><em>Plan Tag</em></a></em> page to view tags assigned to the plan tasks in the plan. The number on the icon represents the number of tags that are assigned to the tasks in the plan.</p>
<p>Refer to <a href="../Use_Cases/Use_Tags">Use Tags f</a>or more information.</p></td>
</tr>
<tr class="odd">
<td><p>Rules</p></td>
<td><p>Click to open the <a href="Work_List_Event_Rules"><em>Work List Event Rules</em></a> page to add, edit and delete the rules that are executed for tasks in the plan when work on the task starts or finishes. The number on the icon represents the number of rules registered to the plan.</p>
<p>Refer to <a href="../Use_Cases/Register_Work_List_Event_Rules_for_a_Plan">Register Work List Event Rules</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Validations</p></td>
<td><p>Click to open the <em><a href="Work_List_Event_Validations_H">Work List Event Validations</a></em> page to add, edit and delete the validations that are executed for tasks in the plan when work on the task starts or finishes. The number on the icon represents the number of validations registered to the plan. Refer to <a href="../Use_Cases/Register_WorkList_Event_Validations_Plan">Register Work List Event Validations</a> for more information.</p></td>
</tr>
</tbody>
</table>

## <span id="Plan_V"></span>Plan V

[Plan H](Plan_H)

<div class="use">

Use this page to [Organize Projects with
Plans](../Use_Cases/Organize_Plans_with_Projects).

</div>

This page has the following tabs:

  - [General](#General_Tab)
  - [Plan](#Plan_Tab)
  - [Status Configuration](#tatus_Configuration_Tab)
  - [Additional Information](#Additional_Information_Tab)
  - [Security](#Security_Tab)
  - [Archive](#Archive_Tab)

## <span id="General_Tab"></span>General tab

Field

Description

Name

Displays the plan name.

Require Comment

Displays an option to indicate if users are required to enter a comment
when finishing a task after the planned finish date. Users finish a task
by clicking Next Action on the Work List when a task status is In
Progress. Values are:

  - **Inherit** – The Require Comment setting is inherited from the most
    granular level in the hierarchy. If the Require Comment setting is
    set to\[None\], Inherit is used by default. The requirement
    hierarchy’s most granular level is task, followed by tag, plan and
    parameter.  
    Require Comment settings set at the task level override those set at
    any other level. If a task's Require Comment setting is set
    to\[None\]or Inherit, the task's Require Comment setting is
    inherited from the tag level (provided the tag level does not also
    have a Require Comment setting of\[None\]or Inherit). If the tag
    level has a Require Comment setting of Inherit or\[None\], Require
    Comment settings are then inherited at the plan level (provided the
    plan level does not also have a Require Comment setting of\[None\]or
    Inherit), and so on.  
    For example, the Require Comment list box has been set to\[None\]at
    the parameter level. At the plan level, it has been set to Inherit.
    At the tag level, the Require Comment list box is set to Yes. At the
    task level, Task A in the Plan has a Require Comment setting of
    Inherit. Task B in the plan has a Require Comment setting of No. In
    this scenario, Task A would have a Require Comment setting of Yes.
    Task B would have a Require Comment setting of No. 
  - **Yes** – This task will require a comment when the user clicks Next
    Action on the Work List after the planned finish date.
  - **No** – This task will not require a comment when the user clicks
    Next Action on the Work List after the planned finish date.

Require Late Comment

Displays an option to indicate if users are required to enter a late
comment when finishing a task after the planned finish date. Users
finish a task by clicking Next Action on the Work List when a task
status is In Progress. Values are:

  - **Inherit** – The Require Late Comment setting is inherited from the
    most granular level in the hierarchy. If the Require Late Comment
    setting is set to\[None\], Inherit is used by default. The
    requirement hierarchy’s most granular level is task, followed by
    tag, plan and parameter.  
    Require Late Comment settings set at the task level override those
    set at any other level. If a task's Require Late Comment setting is
    set to\[None\]or Inherit, the task's Require Late Comment setting is
    inherited from the tag level (provided the tag level does not also
    have a Require Late Comment setting of\[None\]or Inherit). If the
    tag level has a Require Late Comment setting of Inherit or\[None\],
    Require Late Comment settings are then inherited at the plan level
    (provided the plan level does not also have a Require Late Comment
    setting of\[None\]or Inherit), and so on.  
    For example, the Require Late Comment list box has been set
    to\[None\]at the parameter level. At the plan level, it has been set
    to Inherit. At the tag level, the Require Late Comment list box is
    set to Yes. At the task level, Task A in the Plan has a Require Late
    Comment setting of Inherit. Task B in the plan has a Require Late
    Comment setting of No. In this scenario, Task A would have a Require
    Late Comment setting of Yes. Task B would have a Require Late
    Comment setting of No. 
  - **Yes** – This task will require a late comment when the user clicks
    Next Action on the Work List after the planned finish date.
  - **No** – This task will not require a late comment when the user
    clicks Next Action on the Work List after the planned finish date.

Default Calendar

Displays the calendar used for the schedule status calculations for the
selected plan. Refer to [Use a
Calendar](../../Common/Use_Cases/Use_a_Calendar) for more
information.

Attachments

Click to open the *[Attachments](Attachments)* page to upload files
and to download and view files that have been uploaded. Refer to [Upload
Files for a Plan, Task or Work List
Item](../Use_Cases/UpldFilesfoProjTaskWrkListItem) for more
information.

Audit Information

Planned Start Date

Displays the earliest start date of all tasks in the plan according to
the project schedule.

Planned Finish Date

Displays the latest finish date of all tasks in the plan according to
the project schedule.

Actual Start Date

Displays the earliest date work on all tasks began in the plan. Work
begins for a task when the user clicks Next Action on the Work List for
a task that is in Ready status.

The Actual Start Date may differ from the Planned Start Date.

Work on a task starts when a user clicks Next Action on the Work List
when a task is in Ready or Waiting on Dependency status.

Actual Finish Date

Displays the latest date work on all tasks completed in the plan.

The Actual Finish Date may differ from the Planned Finish Date.

Work on a task finishes when a user clicks Next Action on the Work List
when a task is in a status of In Progress.

### <span id="Plan_Tab"></span>Plan tab

<div class="use">

<span>Use this tab to:</span>

  - [Import a Project
    File](../Use_Cases/Import_the_Project_File_into_dspTrack)
  - [Activate and Deactivate a
    Plan](../Use_Cases/Activate_and_Deactivate_a_Plan)
  - [Calculate the Critical
    Path](../Use_Cases/Calculate_the_Critical_Path_for_a_Plan)
  - [Export a Project File](../Use_Cases/Export_a_Project_File)

</div>

Field

Description

Plan File Type

Displays the type of file imported into dspTrack™ to create the plan.
Values are MSProject 2012 and Excel 2007.

**NOTE**: Before a file can be imported:

  - A Plan File Type option must be selected
  - The Plan File Type selected must correspond to the file type of the
    file being imported.

Refer to [Import a Project File into
dspTrack™](../Use_Cases/Import_Project_Files_into_dspTrack) for
more information.

Plan Actions

Upload

Click to upload a file to import into a plan or click the download icon
to download a project file while exporting a file.

Prior to import, the file type must be selected in the Project File Type
list box on the General tab. Refer to [Import a File into
dspTrack™](../Use_Cases/Import_Project_Files_into_dspTrack) for
more information.

Import

Click to import an uploaded file into dspTrack™.

Refer to [Import a File into
dspTrack™](../Use_Cases/Import_Project_Files_into_dspTrack) for
more information.

Deactivate/Activate Plan

Click to activate or deactivate a plan, The label for this field
displays Activate or Deactivate according to the plan’s current state.
The tasks in an active plan display on the Work List and work on these
tasks can be tracked. Tasks in an inactive plan do not display on the
Work List and work on these tasks cannot be tracked.

Refer to [Activate and Deactivate a
Plan](../Use_Cases/Activate_and_Deactivate_a_Plan) for more
information.

Calculate

Click to recalculate the Critical Path for the plan, taking into account
the current Critical Path of the project in MSProject.

**NOTE**: This feature is available for plans based on MSProject files
only. If the Project File Type is Excel 2007, this icon is disabled.

**NOTE**: This button is disabled if:

  - No tasks have been added to the plan
  - The tasks in this plan were added using an Excel import.

**NOTE**: If a project was created in dspTrack and is to be exported, it
must be exported before the critical path has been calculated (i.e.,
before the Calculate icon is clicked on the Plan tab of the Plan page's
Vertical View).

Export

Click to export the plan into an Excel file or an MSProject file. Refer
to [Export a Project File](../Use_Cases/Export_a_Project_File) for
more information.

### <span id="tatus_Configuration_Tab"></span>Status Configuration tab

<div class="use">

Use this tab to [Set Parameters for Schedule Status
Calculation](../Use_Cases/Set_Parameters_for_Schedule_Status_Calculation).

</div>

Field

Description

Schedule Status Outlook ID

Displays an option indicating whether any task’s schedule status in the
plan can improve or cannot improve. Values are:

  - **Optimistic** – A task’s schedule status can improve. For example,
    a task passes the Post-Start Warn threshold and its schedule status
    icon is red. Work on the task begins. The schedule status icon for
    the task changes to green.
  - **Pessimistic** – A task’s schedule status cannot improve. The
    schedule status either does not change or become worse. For example,
    if work on a task has not started and the Pre Start Warn threshold
    has passed, the schedule status icon for that task is yellow.
    Depending on how work proceeds on the task, the task’s scheduled
    status icon remains yellow or changes to red, but will never be
    green, even if the task is back on schedule.

Warning Thresholds (%)

Pre Start

Displays a value that represents a percentage calculation. If work has
not started on a task (the task is in Ready or Waiting on Dependency
status), the Pre Start Warn Threshold sets the point in time prior to
the planned start date that the task’s schedule status is behind and its
Schedule Status icon is yellow.

Refer to [Set Parameters for Schedule Status
Calculation](../Use_Cases/Set_Parameters_for_Schedule_Status_Calculation)
for more information.

Post Start

Displays a value that represents a percentage calculation. If work on
the task has not started, the Post Start Warn Threshold sets the point
in time after the planned start date that the task’s schedule status is
late and its Schedule Status icon is red.

Refer to [Set Parameters for Schedule Status
Calculation](../Use_Cases/Set_Parameters_for_Schedule_Status_Calculation)
for more information.

Pre End

Displays a value that represents a percentage calculation.

If work has started on a task (the task is in In Progress status), the
Pre End Warn Threshold sets the point in time prior to the planned
finish date that the task’s schedule status is behind and its Schedule
Status icon is yellow.

Refer to [Set Parameters for Schedule Status
Calculation](../Use_Cases/Set_Parameters_for_Schedule_Status_Calculation)
for more information.

Post End

Displays a value that represents a percentage calculation.

If work on the task has started (the task is in In Progress status), the
Post End Warn Threshold sets the point in time after the planned finish
date that the task’s schedule status is late and its Schedule Status
icon is red.

Refer to [Set Parameters for Schedule Status
Calculation](../Use_Cases/Set_Parameters_for_Schedule_Status_Calculation)
for more
information.

### <span id="Additional_Information_Tab"></span>Additional Information tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Predecessor Dependency</p></td>
<td><p>Click to open the <em><a href="Project_Dependency">Project Dependency</a></em> page to view dependency relationships for successor tasks in the plan. Other tasks in the plan depend on these tasks to either start or complete (depending on the Dependency Type).</p>
<p><strong>NOTE</strong>: A predecessor dependency can affect Task Status on the Work List. Refer to <a href="../Use_Cases/Use_Dependency_Types">Use Dependency Type</a>s for more information.</p>
<p>The number on this icon is the number of tasks that have a predecessor dependency in the plan.</p>
<p>Dependencies are set at the task level on the <em><a href="Plan_Task_Dependency"><em>Plan Task Dependency</em></a></em> page.</p></td>
</tr>
<tr class="odd">
<td><p>Successor Dependency</p></td>
<td><p>Click to open the <em><a href="Project_Dependency"><em>Project Dependency</em></a></em> page to view dependency relationships for dependent tasks in the plan. Other tasks in the plan must either start or complete (depending on the Dependency Type) before dependent tasks in the plan can start or complete.</p>
<p><strong>NOTE</strong>: A successor Dependency can affect Task Status on the Work List. Refer to <a href="../Use_Cases/Use_Dependency_Types">Use Dependency Types</a> for more information.</p>
<p>Dependencies are set at the task level on the <em><a href="Plan_Task_Dependency">Plan Task Dependency</a></em> page.</p>
<p>The number on this icon is the number of tasks that have a successor dependency in the plan.</p>
<p>Dependencies are set at the task level on the <em>Plan Task Dependency</em> page.</p></td>
</tr>
<tr class="even">
<td><p>Late Tasks</p></td>
<td><p>Click to open the <em><a href="Late_Task">Late Task</a></em> page to view tasks that are late based on the project plan, warn thresholds and other factors. Refer to <a href="../Use_Cases/View_Late_Tasks">View Late Tasks</a> for more information.</p>
<p>The number on this icon is the number of late tasks in the plan.</p>
<p><strong>NOTE</strong>: The icon always displays red, even if there are no late tasks in the plan.</p></td>
</tr>
</tbody>
</table>

### <span id="Security_Tab"></span>Security tab

|                             |                                                                                                                                                                                                                                                                                                                                                                   |
| --------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                       | Description                                                                                                                                                                                                                                                                                                                                                       |
| Setup                       | Click to open the *[Plan Access Setup](Project_Access_Setup)* page to grant users permission to make updates to the plan or to restrict users to read only access. Refer to [Set Plan Security](../Config/Set_Plan_Security) for more information.                                                                                                        |
| Register Unregistered Users | Click to open the *[Plan User Registration](Plan_User_Registration)* page to register users who were imported into dspTrack™ along with a project file, but who do not have user accounts in the platform. Refer to [Register Unregistered Users Imported into dspTrack™](../Use_Cases/Register_Unregistered_Users_Imprtd_dspTrack) for more information. |

### <span id="Archive_Tab"></span>Archive tab

<div class="use">

Use this page to [Archive a
Plan](../Use_Cases/Archive_a_Plan).

</div>

|                    |                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field              | Description                                                                                                                                                                      |
| Last Archived On   | Displays the last archived date (i.e., the last time the user in the Last Archived By field clicked Create New Archive).                                                         |
| Last Archived By   | Displays the user ID of the last user who clicked Create New Archive.                                                                                                            |
| Create New Archive | Click to create an archive. dspTrack™ stores a copy of that plan and the date the archive was saved in an archive table, and the data can then be used as the basis for reports. |
