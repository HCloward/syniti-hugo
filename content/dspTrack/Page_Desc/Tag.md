+++
title = ''
solution = 'Platform'
+++

# <span id="_Toc378151421"></span>Tag H (Also Tag – All Types)

<div class="use">

Use this page to [Add a Tag](../Use_Cases/Add_a_Tag.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Track \>
    </span>**Configuration \> Tag Type** from the *Navigation* pane.
2.  Click the icon for a Tag Type.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Copy Tag Tasks</p></td>
<td><p>Click to open the <em><a href="Copy_Tag.htm">Copy Tag Tasks</a></em> page to copy all tasks to which this tag has been assigned to a plan specified on the <em>Copy TagTasks</em> page.</p></td>
</tr>
<tr class="odd">
<td><p>NAME</p></td>
<td><p>Displays the tag name.</p></td>
</tr>
<tr class="even">
<td><p>Tag Type</p></td>
<td><p>Displays an icon that represents the tag type.</p></td>
</tr>
<tr class="odd">
<td><p>TYPE</p></td>
<td><p>Displays the name of the tag type associated with the tag. Options are Logic, Plan and Security.</p></td>
</tr>
<tr class="even">
<td><p>PLANNED START DATE</p></td>
<td><p>Displays the earliest planned start date of a task assigned to the tag according to the project plan.</p></td>
</tr>
<tr class="odd">
<td><p>PLANNED FINISH DATE</p></td>
<td><p>Displays the latest planned finish date of a task assigned to the tag according to the project plan.</p></td>
</tr>
<tr class="even">
<td><p>Plans</p></td>
<td><p>Click to open the <em><a href="Plan_Tag.htm">Plan Tag</a></em> page to view a list of all plans that use the selected tag.</p></td>
</tr>
<tr class="odd">
<td><p>Tasks</p></td>
<td><p>Click to open the <em><a href="Plan_Task_Tag.htm">Plan Task Tag</a></em> page to view a list of all plan tasks or plans assigned to the tag.</p></td>
</tr>
<tr class="even">
<td><p>Assign to Tasks</p></td>
<td><p>Click to open the <em><a href="Tag_Plan_Task_Assignment.htm"><em>Tag Plan Task Assignment</em></a></em> page to add tasks to and remove tasks from the selected tag.</p></td>
</tr>
<tr class="odd">
<td><p>Registrations</p></td>
<td><p>Click to open the <em><a href="Security_Tag.htm">Security Tag</a></em> page or the <em>Logic Tag</em> page, depending on the Tag Type selected. Security tags can have users assigned, Logic tags can have validations and rule assigned.</p>
<p><strong>NOTE</strong>: This icon is disabled for tags with a tag type of Plan.</p></td>
</tr>
</tbody>
</table>

## <span id="Tag_V"></span>Tag V (Also Tag – All Types)

<div class="use">

Use this page to:

  - [Add a Tag](../Use_Cases/Add_a_Tag.htm)
  - [Add Comment Requirements for
    Tasks](../Use_Cases/Set_Comment_Requirements_for_Tasks.htm)

</div>

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Name</p></td>
<td><p>Displays the tag name.</p></td>
</tr>
<tr class="odd">
<td><p>Description</p></td>
<td><p>Displays a description of the tag.</p></td>
</tr>
<tr class="even">
<td><p>Planned Start Date</p>
<p> </p></td>
<td><p>Displays the earliest planned start date of any tasks to which the tag is assigned according to the project plan.</p></td>
</tr>
<tr class="odd">
<td><p>Planned Finish Date</p>
<p> </p></td>
<td><p>Displays the latest planned finish date of any tasks to which the tag is assigned according to the project plan.</p></td>
</tr>
<tr class="even">
<td><p>Actual Start Date</p>
<p> </p></td>
<td><p>Displays the earliest actual start date work began for any tasks to which the tag is assigned which may differ from the planned start date</p></td>
</tr>
<tr class="odd">
<td><p>Actual Finish Date</p>
<p> </p></td>
<td><p>Displays the latest actual finish date work began for any tasks to which the tag is assigned which may differ from the planned finish date.</p>
<p>This field does not display a date until all tasks associated with this tag are complete. A task is complete when a user clicks Next Action on the Work List for a task with a status of In Progress. If a new task is added to the tag after all tasks have been completed, this field updates to blank.</p></td>
</tr>
<tr class="even">
<td><p>Require Late Comment</p></td>
<td><p>Displays an option to indicate if users are required to enter a late comment when finishing a task assigned to the tag after the planned finish date. Users finish a task by clicking Next Action on the Work List when a task status is In Progress. Values are:</p>
<ul>
<li><strong>Inherit</strong> - The Require Comment setting is inherited from the most granular level in the hierarchy. If the Require Comment setting is set to [None], Inherit is used by default. The requirement hierarchy’s most granular level is task, followed by tag, plan and parameter.<br />
Require Comment settings set at the task level override those set at any other level. If a task's Require Comment setting is set to [None] or Inherit, the task's Require Comment setting is inherited from the tag level (provided the tag level does not also have a Require Comment setting of [None] or Inherit). If the tag level has a Require Comment setting of Inherit or [None], Require Comment settings are then inherited at the plan level (provided the plan level does not also have a Require Comment setting of [None] or Inherit), and so on.<br />
For example, the Require Comment list box has been set to [None] at the parameter level. At the plan level, it has been set to Inherit. At the tag level, the Require Comment list box is set to Yes. At the task level, Task A in the Plan has a Require Comment setting of Inherit. Task B in the plan has a Require Comment setting of No. In this scenario, Task A would have a Require Comment setting of Yes. Task B would have a Require Comment setting of No. </li>
<li><strong>Yes</strong> - This task will require a comment when the user clicks Next Action on the Work List after the planned finish date.</li>
<li><strong>No</strong> - This task will not require a comment when the user clicks Next Action on the Work List after the planned finish date.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Require Comment</p></td>
<td><p>Settings set at the task level override those set at any other level. If a task's Require Comment setting is set to [None] or Inherit, the task's Require Comment setting is inherited from the tag level (provided the tag level does not also have a Require Comment setting of [None] or Inherit). If the tag level has a Require Comment setting of Inherit or [None], Require Comment settings are then inherited at the plan level (provided Displays an option to indicate if users are required to enter a comment when finishing a task assigned to the tag after the planned finish date. Users finish a task by clicking Next Action on the Work List when a task status is In Progress. Values are:</p>
<ul>
<li><strong>Inherit</strong> - The Require Comment setting is inherited from the most granular level in the hierarchy. If the Require Comment setting is set to [None], Inherit is used by default. The requirement hierarchy’s most granular level is task, followed by tag, plan and parameter.<br />
Require Comment the plan level does not also have a Require Comment setting of [None] or Inherit), and so on.<br />
For example, the Require Comment list box has been set to [None] at the parameter level. At the plan level, it has been set to Inherit. At the tag level, the Require Comment list box is set to Yes. At the task level, Task A in the Plan has a Require Comment setting of Inherit. Task B in the plan has a Require Comment setting of No. In this scenario, Task A would have a Require Comment setting of Yes. Task B would have a Require Comment setting of No. </li>
<li><strong>Yes</strong> - This task will require a comment when the user clicks Next Action on the Work List on or before the planned finish date.</li>
<li><strong>No</strong> - This task will not require a comment when the user clicks Next Action on the Work List on or before the planned finish date.</li>
</ul></td>
</tr>
</tbody>
</table>
