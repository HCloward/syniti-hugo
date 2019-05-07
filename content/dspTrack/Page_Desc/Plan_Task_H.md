+++
title = 'Plan Task H'
solution = 'Platform'
+++

# Plan Task H

[Plan Task V](#Plan_Task_V)

<div class="use">

Use this page to [Add a Plan
Task](../Use_Cases/Add_a_Plan_Task_Manually.htm).

</div>

<span style="font-weight: bold;">NOTE:</span> Bulk Execution has been
enabled on this page. Refer to [Use Bulk
Execution](../../Bulk_Exec/Use_Bulk_Execution.htm) for more information.

To access this page:

1.  Click **Track \> Project** in Navigation pane.
2.  Click **Plans** for a project.
3.  Click **Tasks** for a Plan.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Copy Plan Task</p></td>
<td><p>Click to open the <em><a href="../Use_Cases/Copy_Plan_Task.htm">Copy Plan Task</a></em> page to copy the selected task to use as the basis for a new task.</p></td>
</tr>
<tr class="odd">
<td><p>SCHEDULE STATUS</p></td>
<td><p>Displays an image related to the task’s schedule status, which is calculated by dspTrack™. Options are:</p>
<ul>
<li><strong>Green</strong> – the task is on time according to the schedule.</li>
<li><strong>Yellow</strong> – the task has reached a threshold set to indicate that the task is in danger of being late.</li>
<li><strong>Red</strong> – the task is late. If a given task is part of the critical path for a project, and a task before it in the critical path is late, then this given task will also display as late.</li>
</ul>
<p>Refer to <a href="../Use_Cases/Set_Parameters_for_Schedule_Status_Calculation.htm">Set Parameters for Schedule Status Calculation</a> for more information</p></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the task name.</p></td>
</tr>
<tr class="odd">
<td><p>TASK STATUS</p></td>
<td><p>Displays the status of the task in the workflow. Values are Ready, Waiting on Dependency, In Progress and Completed.</p>
<p>Refer to <a href="Task_Status1.htm">Task Status</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>PLANNED START DATE</p></td>
<td><p>Displays the date work on the task should start according to the project plan.</p></td>
</tr>
<tr class="odd">
<td><p>PLANNED FINISH DATE</p></td>
<td><p>Display the date work on the task should end according to the project plan.</p></td>
</tr>
<tr class="even">
<td><p>DURATION</p></td>
<td><p>Displays the number related to the Unit of Measure that defines how long the task should take to complete. This number can be a decimal and is used in schedule status calculations and on reports.</p>
<p>This field must be greater than 0.</p></td>
</tr>
<tr class="odd">
<td><p>UOM</p></td>
<td><p>Displays the Unit of Measure. Combined with the duration, this determines how long work on a task should take and is used in schedule status calculations and on reports.</p></td>
</tr>
<tr class="even">
<td><p>Users</p></td>
<td><p>Click to open the <em><a href="Plan_Task_User.htm">Plan Task User</a></em> page to assign resources to the task. The number on this icon is the number of users assigned to the task.</p></td>
</tr>
<tr class="odd">
<td><p>Predecessor Tasks</p></td>
<td><p>Click to open the <em><a href="Plan_Task_Dependency.htm">Plan Task Dependency</a></em> page to set up predecessor and successor relationships for the task. Refer to Use <a href="../Use_Cases/Use_Dependency_Types.htm">Dependency Types</a> for more information.</p>
<p>The number on this icon is the number of tasks that have a predecessor dependency with the selected task.</p></td>
</tr>
<tr class="even">
<td><p>Assign Tags</p></td>
<td><p>Click to open the <em><a href="Plan_Task_Tag_Assignment.htm">Plan Task Tag Assignment</a></em> page to assign tags to and remove tags from the selected task. Refer to <a href="../Use_Cases/Assign_a_Tag_to_Tasks.htm">Assign a Tag to Tasks</a> for more information.</p>
<p>The number on this icon is the number of tags assigned to the selected task.</p></td>
</tr>
<tr class="odd">
<td><p>Rules</p></td>
<td><p>Click to open the <em><a href="Work_List_Event_Rule%20Plan_Task.htm"><em>Work List Event Rule– Plan Task</em></a></em> page to add, edit and delete the rules that are executed for the task when work on the task starts or finishes.</p>
<p>The number on this icon is the number of rules that have been added for the selected task.</p></td>
</tr>
<tr class="even">
<td><p>Validations</p></td>
<td><p>Click to open the <em><a href="Work_List_Event_Validations_Plan_Task.htm">Work List Event Validations-Plan Task</a></em> page to add, edit and delete the validations that are executed for the task when work on the task starts or finishes.</p>
<p>The number on this icon is the number of validations that have been added for the selected task.</p></td>
</tr>
</tbody>
</table>

## <span id="Plan_Task_V"></span>Plan Task V

[Plan Task H](Plan_Task_H.htm)

This page has the following tabs:

  - [General](#General_Tab)
  - [Additional Information](#Additional_Information_Tab)

### <span id="General_Tab"></span>General tab

<div class="use">

Use this tab to

  - [Set Comment Requirements for
    Tasks](../Use_Cases/Set_Comment_Requirements_for_Tasks.htm)
  - [Add a Comment to a Task](../Use_Cases/Add_a_Comment_to_a_Task.htm)

</div>

Field

Description

Name

Displays the task name.

Description

Displays a brief description of the task.

Task Status

Displays the status of the task. Values are Ready, Waiting on
Dependency, In Progress, and Completed. Refer to [Task
Status](Task_Status1.htm) for more information.

Planned Start Date

Displays the date work on the task should start according to the project
plan.

Planned Finish Date

Displays the date work on the task should end according to the project
plan.

Documentation

Attachments

Click to open the
<span style="font-style: italic;">[Attachments](Attachments.htm)</span>page
to upload a file and download and view an uploaded file.

Refer to [Upload Files for a Plan, Task or Work List
Item](../Use_Cases/UpldFilesfoProjTaskWrkListItem.htm) and [Download and
View Uploaded Files for a Plan, Task, or Work List
Item](../Use_Cases/DownloadViewUploadedFiles.htm) for more information.

Require Comment

Displays an option to indicate if users are required to enter a comment
when finishing a task after the planned finish date. Users finish a task
by clicking Next Action on the Work List when a task status is In
Progress. Values are:

  - **Inherit –** The Require Comment setting is inherited from the most
    granular level in the hierarchy. If the Require Comment setting is
    set to \[None\], Inherit is used by default. The requirement
    hierarchy’s most granular level is task, followed by tag, plan and
    parameter.  
    Require Comment settings set at the task level override those set at
    any other level. If a task's Require Comment setting is set to
    \[None\] or Inherit, the task's Require Comment setting is inherited
    from the tag level (provided the tag level does not also have a
    Require Comment setting of \[None\] or Inherit). If the tag level
    has a Require Comment setting of Inherit or \[None\], Require
    Comment settings are then inherited at the plan level (provided the
    plan level does not also have a Require Comment setting of \[None\]
    or Inherit), and so on.  
    For example, the Require Comment list box has been set to \[None\]
    at the parameter level. At the plan level, it has been set to
    Inherit. At the tag level, the Require Comment list box is set to
    Yes. At the task level, Task A in the Plan has a Require Comment
    setting of Inherit. Task B in the plan has a Require Comment setting
    of No. In this scenario, Task A would have a Require Comment setting
    of Yes. Task B would have a Require Comment setting of No. 
  - **Yes –** This task will require a comment when the user clicks Next
    Action on the Work List after the planned finish date.
  - **No –** This task will not require a comment when the user clicks
    Next Action on the Work List after the planned finish date.

Comment

Displays a user-entered comment about the task.

Require Late Comment

Displays an option to indicate if users are required to enter a late
comment when finishing a task after the planned finish date. Users
finish a task by clicking Next Action on the Work List when a task
status is In Progress. Values are:

  - **Inherit –** The Require Late Comment setting is inherited from the
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
  - **Yes –** This task will require a comment when the user clicks Next
    Action on the Work List after the planned finish date.
  - **No –** This task will not require a comment when the user clicks
    Next Action on the Work List after the planned finish date.

Late Comment

Click to open the *Item Comment Code* page to add a late comment code
and a comment to the task. Comment codes qualify the late reason for
Plan Tasks, such as Error in Development or Pending Validation. Refer to
[Use Comment Codes](../Use_Cases/Use_Comment_Codes.htm) for more
information.

**NOTE**: Entering a late comment may be required, depending on how
comment requirements for tasks are set. Refer to [Set Comment
Requirements for
Tasks](../Use_Cases/Set_Comment_Requirements_for_Tasks.htm) for more
information.

Audit Information

Actual Start Date

Displays the date work on the task began. This date may be different
from the planned start date.

Work on a task begins when a user clicks Next Action on the Work List
when a task is in Ready status.

Started By

Displays the user ID of the user who clicked Next Action on the Work
List for the task when the task was in Ready status.

Actual Finish Date

Displays the date work on the task finished. This date may be different
from the planned finish date.

Work on a task ends when a user clicks Next Action on the Work List when
a task is in a status of In Progress.

Finished By

Displays the user ID of the user who clicked Next Action on the Work
List for the task when the task was in a status of In
Progress.

### <span id="Additional_Information_Tab"></span>Additional Information tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Critical</p></td>
<td><p>If enabled, the task is on the Critical Path. If this task is late, the schedule status of all other tasks in the Critical Path that are scheduled after this task are also late.</p>
<p>This value can be set manually or when a project file is imported.</p>
<p>Refer to<a href="../Use_Cases/Calculate_the_Critical_Path_for_a_Plan.htm"> Calculate the Critical Path for a Plan</a>  for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Milestone</p></td>
<td><p>If enabled the task is a milestone task.</p></td>
</tr>
<tr class="even">
<td><p>External ID</p></td>
<td><p>Displays the ID that MSProject assigned to the task, and imported with the project file. Use the External Id to search for the task in MSProject. Tasks that were added manually do not have an External ID. If the task was imported as part of an Excel file, this field is blank.</p></td>
</tr>
<tr class="odd">
<td><p>Schedule Status Outlook ID</p></td>
<td><p>Displays an option indicating whether any task’s schedule status in the plan can improve or cannot improve. Values are:</p>
<ul>
<li><strong>Inherit</strong> – The values is inherited from the plan level.</li>
<li><strong>Optimistic</strong> - The task’s schedule status can improve. For example, a task passes the Post-Start Warn threshold and its schedule status icon is red. Work on the task begins. The schedule status icon for the task changes to green.</li>
<li><strong>Pessimistic</strong> - The task’s schedule status cannot improve. The schedule status either does not change or become worse. For example, if work on a task has not started and the Pre Start Warn threshold has passed, the schedule status icon for that task is yellow. Depending on how work proceeds on the task, the task’s scheduled status icon remains yellow or changes to red, but will never be green, even if the task is back on schedule.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Predecessor Tasks</p></td>
<td><p>Click to open the <em><a href="Plan_Task_Dependency.htm">Plan Task Dependency</a></em> page to add, edit and delete dependency relationships for the selected task.</p>
<p><strong>NOTE</strong>: A predecessor dependency can affect Task Status on the Work List. Refer to <a href="../Use_Cases/Use_Dependency_Types.htm">Use Dependency Types</a> for more information.</p>
<p>The number on this icon is the number of tasks that have a predecessor dependency with the selected task.</p>
<p>View dependencies for all tasks in the plan on the <em>Project Dependency</em> page.</p></td>
</tr>
<tr class="odd">
<td><p>Successor Tasks</p></td>
<td><p>Click to open <em><a href="Plan_Task_Dependency_Successor.htm">Plan Task Dependency Successor</a></em> page to view a list of successor tasks related to the selected task.</p>
<p><strong>NOTE</strong>: A successor Dependency can affect Task Status on the Work List. Refer to <a href="../Use_Cases/Use_Dependency_Types.htm">Use Dependency Types</a> for more information.</p>
<p>View dependencies for all tasks in the plan on the <em>Project Dependency</em> page.</p></td>
</tr>
</tbody>
</table>
