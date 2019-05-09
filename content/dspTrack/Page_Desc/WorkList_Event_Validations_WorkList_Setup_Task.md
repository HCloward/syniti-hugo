+++
title = 'Work List Event Validations -  Work List Setup Task H'
solution = 'Platform'
+++

# Work List Event Validations -  Work List Setup Task H

[Work List Event Validations - Work List Setup Task
V](#Work_List_Event_Validations_-_Work_List_Setup_Task__V)

<div class="use">

Use this page to view Work List Event Validations assigned to Plan Tasks
accessed from the *[Work List Setup](Work_List_Setup_H)* page.

</div>

Refer to [Register Work List Event Validations for Work List
Items](../Use_Cases/Register_WorkList_Event_Valid_WorkList_Item) for
more information.

To access this page:

1.  Select <span style="font-weight: bold;">Track
    \></span><span style="font-family: Arial, sans-serif;">
    **Configuration \> Work List** in the *Navigation* pane.</span>
2.  Click **Validations** for a Work List Item while a Plan Task is
    selected.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>WORK LIST ITEM ID</p></td>
<td><p>Displays the name of the work list item.</p></td>
</tr>
<tr class="odd">
<td><p>PLAN TASK ID</p></td>
<td><p>Displays the Plan Task associated with the validation.</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the validation runs if multiple validations are assigned to the Plan Task.</p></td>
</tr>
<tr class="odd">
<td><p> DATA SOURCE ID</p></td>
<td><p>Displays the name of the data source that stores the validation.</p></td>
</tr>
<tr class="even">
<td><p>VALIDATION TYPE</p></td>
<td><p>Displays whether the validation is a stored procedure or a view.</p></td>
</tr>
<tr class="odd">
<td><p>WORK LIST EVENT ID</p></td>
<td><p>Displays the event that triggers the validation to run. Values are:</p>
<ul>
<li><strong>Finish</strong> – The validation runs when a user completes the Plan Task on the Work List by clicking Next Action when the Plan Task has a status of In Progress.</li>
<li><strong>Start</strong> – The validation runs when a user starts work on the Plan Task on the Work List by clicking Next Action when the Plan Task has a status of Ready.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the validation name.</p></td>
</tr>
<tr class="odd">
<td><p>ACTIVE</p></td>
<td><p>If enabled, the validation is active. If disabled, the validation is inactive and will not run.</p></td>
</tr>
<tr class="even">
<td><p>TAG ID</p></td>
<td><p>Displays the name of the tag used by the task to assign the validation. If the validation is assigned directly to a Task or Plan (without using a tag), then this field is empty.</p>
<p>Refer to <a href="../Use_Cases/Configure_Logic_Tags">Configure Logic Tags</a> for more information.</p></td>
</tr>
</tbody>
</table>

## <span id="Work_List_Event_Validations_-_Work_List_Setup_Task__V"></span>Work List Event Validations - Work List Setup Task  V

[Horizontal View](WorkList_Event_Validations_WorkList_Setup_Task)

<div class="use">

Use this page to view Work List Event Validations assigned to Plan Tasks
accessed from the *[Work List Setup](Work_List_Setup_H)* page.

</div>

Refer to [Register Work List Event Validations for Work List
Items](../Use_Cases/Register_WorkList_Event_Valid_WorkList_Item) for
more information.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Project ID</p></td>
<td><p>Displays the project to which the plan task belongs.</p></td>
</tr>
<tr class="odd">
<td><p>Plan Task ID</p></td>
<td><p>Displays the Plan Task associated with the validation.</p></td>
</tr>
<tr class="even">
<td><p>Work List Item ID</p></td>
<td><p>Displays the work list item name.</p></td>
</tr>
<tr class="odd">
<td><p>Tag ID</p></td>
<td><p>Displays the name of the tag to which the validation is assigned. If the validation is assigned directly to a Task or Plan (without using a tag), then this field is empty.</p>
<p>Refer to <a href="../Use_Cases/Configure_Logic_Tags">Configure Logic Tags</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Configuration</p></td>
<td><p>Displays the configuration ID.</p></td>
</tr>
<tr class="odd">
<td><p>Priority</p></td>
<td><p>Displays the order the validation runs if multiple validations are assigned to the Plan Task.</p></td>
</tr>
<tr class="even">
<td><p>Data Source ID</p></td>
<td><p>Displays the name of the data source that stores the validation.</p></td>
</tr>
<tr class="odd">
<td><p>View/Procedure</p></td>
<td><p>Displays the validation name. The label on this field depends on the Validation Type selected on the <span style="font-style: italic;">Horizontal</span> View.</p></td>
</tr>
<tr class="even">
<td><p>Work List Event ID</p></td>
<td><p>Displays the event that triggers the validation to run. Values are:</p>
<ul>
<li><strong>Finish</strong> – The validation runs when a user completes the selected task on the Work List by clicking Next Action when the task has a status of In Progress.</li>
<li><strong>Start</strong> – The validation runs when a user starts work on the selected task on the Work List by clicking Next Action after the task has been created.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Active</p></td>
<td><p>If enabled, the validation is active. If disabled, the validation is inactive and will not run.</p></td>
</tr>
<tr class="even">
<td><p>Validation Message</p></td>
<td><p>Displays a brief message that will display to the user when the validation fails.</p></td>
</tr>
<tr class="odd">
<td><p>Description</p></td>
<td><p>Displays a detailed description that will display to the user when the validation fails.</p>
<p><strong>NOTE</strong>: This description should provide information about what may have caused the error and potential solutions if applicable.</p></td>
</tr>
</tbody>
</table>
