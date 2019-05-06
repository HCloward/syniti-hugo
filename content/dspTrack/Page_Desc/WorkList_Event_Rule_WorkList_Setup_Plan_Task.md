# Work List Event Rule - Work List Setup – Plan Task

<div class="use">

Use this page to view Work List Event Rules
<span class="MsoHyperlink">assigned to Plan Tasks accessed from the
*Work List Setup* page.</span>

</div>

Refer to [Register Work List Event Rules for a Work List
Item](../Use_Cases/Register_WorkList_Event_Rules_WorkList_Item.htm) for
more information.

To access this page:

1.  Click <span style="font-weight: bold;">Track \> Configuration \>
    Work List</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Rules</span> icon for a
    Work List Item.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>WORK LIST ITEM ID</p></td>
<td><p>Displays the name of this task as it appears on the Work List.</p>
<p><strong>NOTE</strong>: The Plan Task ID and the corresponding Work List Item ID will always be identical, but they represent data stored in two tables.</p></td>
</tr>
<tr class="odd">
<td><p>PLAN ID</p></td>
<td><p>Displays the name of the plan associated with the rule, or the Plan Task to which the rule is assigned.</p></td>
</tr>
<tr class="even">
<td><p>PLAN TASK ID</p></td>
<td><p>Displays the task name, if the rule is associated with a task.</p>
<p><strong>NOTE</strong>: If the rule was added to a plan, this field is blank.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the rule runs if multiple rules are assigned to the Plan Task.</p></td>
</tr>
<tr class="even">
<td><p>DATA SOURCE ID</p></td>
<td><p>Displays the name of the data source that stores the rule.</p></td>
</tr>
<tr class="odd">
<td><p>RULE</p></td>
<td><p>Displays the rule name.</p></td>
</tr>
<tr class="even">
<td><p>WORK LIST EVENT ID</p></td>
<td><p>Displays the event that triggers the rule to run. Values are:</p>
<ul>
<li><strong>Finish</strong> – The rule runs when a user completes the Plan Task on the Work List by clicking Next Action when the Plan Task status is In Progress.</li>
<li><strong>Start</strong> – The rule runs when a user starts work on the selected task on the Work List by clicking Next Action when the Plan Task status is Ready.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>ACTIVE</p></td>
<td><p>If enabled, the rule is active. If disabled, the rule is inactive and will not run.</p></td>
</tr>
<tr class="even">
<td><p>COMMENT</p></td>
<td><p>Displays a user-entered comment about the rule.</p></td>
</tr>
<tr class="odd">
<td><p>TAG ID</p></td>
<td><p>Displays the name of the tag if the rule was assigned to the task using a tag.</p>
<p>Refer to <a href="../Use_Cases/Configure_Logic_Tags.htm">Configure Logic Tags</a> for more information.</p>
<p><strong>NOTE</strong>: If the rule is assigned directly to a plan or Plan Task (without using a tag), then this field is empty.</p></td>
</tr>
</tbody>
</table>
