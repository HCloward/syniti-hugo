+++
title = 'Work List Event Rule - Plan Task'
solution = 'Platform'
+++

# Work List Event Rule - Plan Task

<div class="use">

Use this page to [Register Work List Event Rules to a Plan
Task](../Use_Cases/Register_Work_List_Event_Rules_for_a_Plan_Task).

</div>

To access this page:

1.  Select **Track \> Project** in the *Navigation* pane.
2.  Click **Plans** for a project.
3.  Click **Tasks** for a plan.
4.  Click **Rules** for a task.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>PLAN TASK ID</p>
<p> </p></td>
<td><p>Displays the task name associated with the rule.</p>
<p><strong>NOTE</strong>: If the rule was added to a Work List Item or to a plan only, this field is blank.</p></td>
</tr>
<tr class="odd">
<td><p>PLAN ID</p></td>
<td><p>Displays the name of the plan associated with the selected task, or the name of the plan to which the rule was added.</p>
<p><strong>NOTE</strong>: If the rule was added to a Work List Item, this field is blank.</p></td>
</tr>
<tr class="even">
<td><p>WORK LIST ITEM ID</p></td>
<td><p>Displays the name of the Work List Item associated with the rule.</p>
<p><strong>NOTE</strong>: If the rule was added to a Plan Task or a plan, this field is blank.</p></td>
</tr>
<tr class="odd">
<td><p>TAG ID</p></td>
<td><p>Displays the name of the tag to which the rule is assigned if it was added to the task using a tag. Refer to <a href="../Use_Cases/Configure_Logic_Tags">Configure Logic Tags</a> for more information.</p>
<p><strong>NOTE</strong>: If the rule is assigned directly to a Plan Task, Work List Item, or plan (without using a tag), then this field is blank.</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the rule runs if multiple rules are assigned to the selected Plan Task, plan, or Work List item.</p></td>
</tr>
<tr class="odd">
<td><p>DATA SOURCE ID</p></td>
<td><p>Displays the name of the data source that stores the rule.</p></td>
</tr>
<tr class="even">
<td><p>RULE</p></td>
<td><p>Displays the rule name.</p></td>
</tr>
<tr class="odd">
<td><p>WORK LIST EVENT ID</p></td>
<td><p>Displays the event that triggers the rule to run. Values are:</p>
<ul>
<li> <strong>Finish</strong> – The rule runs when a user completes the Plan Task on the Work List by clicking Next Action when the task’s status is In Progress.</li>
<li><strong>Start</strong> – The rule runs when a user starts work on the Plan Task on the Work List by clicking Next Action when the task’s status is Ready.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If enabled, the rule is active. If disabled, the rule is inactive and will not run.</p></td>
</tr>
<tr class="odd">
<td><p>COMMENT</p></td>
<td><p>Displays a user-entered comment about the rule.</p></td>
</tr>
</tbody>
</table>
