+++
title = 'Parameters'
solution = 'Platform'
+++

# Parameters

<div class="use">

This page has the following tabs:

  - [Validations](#Validations_Tab)
  - [Workflow](#Work_Flow_Tab)
  - [Security](#Security_Tab)

</div>

### <span id="Validations_Tab"></span>Validations tab

Use this tab to [Create Comment Requirements for
Tasks](../Use_Cases/Set_Comment_Requirements_for_Tasks).

To access this page, select **Track \> Configuration \>
Parameters** from *Navigation* pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Require Comment</p></td>
<td><p>Displays an option to indicate if users are required to enter a comment when finishing a task after the planned finish date. Users finish a task by clicking Next Action on the Work List when a task status is In Progress. Values are:</p>
<ul>
<li><strong>Yes</strong> – This task will require a comment when the user clicks Next Action on the Work List to move the Plan Task from In Progress status to Completed after the planned finish date.</li>
<li><strong>No</strong> – This task will not require a comment when the user clicks Next Action on the Work List to move the Plan Task from In Progress status to Completed after the planned finish date.</li>
</ul>
<p>This setting can be overwritten at the plan, tag, and task level.</p>
<p>Refer to <a href="../Use_Cases/Set_Comment_Requirements_for_Tasks">Set Comment Requirements for Tasks</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Require Late Comment</p></td>
<td><p>Displays an option to indicate if users are required to enter a late comment when finishing a task after the planned finish date. Users finish a task by clicking Next Action on the Work List when a task status is In Progress. Values are:</p>
<ul>
<li><strong>Yes</strong> – This task will require a late comment when the user clicks Next Action on the Work List to move the Plan Task from In Progress status to Completed after the planned finish date.</li>
<li><strong>No</strong> – This task will not require a late comment when the user clicks Next Action on the Work List to move the Plan Task from In Progress status to Completed after the planned finish date.</li>
</ul>
<p>This setting can be overwritten at the plan, tag, and task level.</p>
<p>Refer to <a href="../Use_Cases/Set_Comment_Requirements_for_Tasks">Set Comment Requirements for Tasks</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Default Plan Calendar</p></td>
<td><p>Displays the name of the calendar used by default when an MSProject file or an Excel file are imported into dspTrack™. The calendar is used in schedule status calculations.</p>
<p>Refer to <a href="../../Common/Use_Cases/Use_a_Calendar">Use a Calenda</a>r for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Plan Upload File Path</p></td>
<td><p>Displays the file path where project files (MSProject files or Excel files) are stored once uploaded during the import process. Refer to <a href="../Use_Cases/Import_Project_Files_into_dspTrack">Import a Project File into dspTrack™</a> for more information.</p>
<p><strong>NOTE</strong>: This field must be completed on a client’s site, and is required before a project file can be uploaded into dspTrack™. Refer to <a href="../Use_Cases/Set_the_Upload_Path_for_dspTrack">Set the Upload Path for dspTrack™</a> for more information.</p></td>
</tr>
</tbody>
</table>

### <span id="Work_Flow_Tab"></span>Workflow tab

Use this page to set a value that controls how long a user can [View
Workflow Messages
Sent](../Use_Cases/View_Workflow_Messages_Sent).

|                         |                                                                                                                                                                                                                                                                                                                              |
| ----------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                   | Description                                                                                                                                                                                                                                                                                                                  |
| Workflow Retention Days | Displays the number of days Workflow notifications are retained and can be viewed on the <span style="font-style: italic;">[Workflow Log](Work_Flow_Log)</span> page. Notifications include Escalation process emails, messages about tasks that are in a Ready status, or messages about tasks that have fallen behind. |

### <span id="Security_Tab"></span>Security tab

|                              |                                                                                                                                                                                      |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field                        | Description                                                                                                                                                                          |
| Plan User Access Sync Enable | If enabled, DSP users who have access to dspTrack (via Roles or Security Definitions) will be added into dspTrack ttProjectAccessSetup tables to facilitate Project task assignment. |
