+++
title = 'Work List Event Validations H'
solution = 'Platform'
+++

# Work List Event Validations H

[Work List Event Validations V](#Work_List_Event_Validations_V)

<div class="use">

Use this page to [Register Work List Event Validations to a
Plan](../Use_Cases/Register_WorkList_Event_Validations_Plan).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Track \>
    </span>**Project** in the *Navigation* pane.
2.  Click **Plans** for a project.
3.  Click **Validations** for a plan.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>PLAN TASK ID</p></td>
<td><p>Displays the name of the Plan Task associated with the validation if the validation was added at the Plan Task level.</p>
<p>If the validation was added at the plan level, this field is blank.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the validation runs if multiple validations are assigned to the plan.</p></td>
</tr>
<tr class="even">
<td><p>VALIDATION TYPE</p></td>
<td><p>Displays whether the validation is a stored procedure or a view.</p></td>
</tr>
<tr class="odd">
<td><p>DATA SOURCE ID</p></td>
<td><p>Displays the name of the data source that stores the validation.</p></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the validation name.</p></td>
</tr>
<tr class="odd">
<td><p>WORK LIST EVENT ID</p></td>
<td><p>Displays the event that triggers the validation to run. Values are:</p>
<ul>
<li><strong>Finish</strong> – The validation runs when a user completes the a Plan Task for the plan on the Work List by clicking Next Action when the task has a status of In Progress.</li>
<li><strong>Start</strong> – The validation runs when a user starts work on a Plan Task in the plan on the Work List by clicking Next Action after the task has been created.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If enabled, the validation is active. If disabled, the validation is inactive and will not run.</p></td>
</tr>
<tr class="odd">
<td><p>TAG ID</p></td>
<td><p>Displays the name of the tag used to assign the Plan Task to the validation. If the validation is assigned directly to a plan or Plan Task (without using a tag), then this field is empty.</p></td>
</tr>
</tbody>
</table>

## <span id="Work_List_Event_Validations_V"></span>Work List Event Validations V

[Work List Event Validations H](Work_List_Event_Validations_H)

<div class="use">

Use this page to [Register Work List Event Validations to a
Plan](../Use_Cases/Register_WorkList_Event_Validations_Plan).

</div>

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Plan Task ID</p></td>
<td><p>Displays the name of the Plan Task associated with the validation if the validation was added at the Plan Task level.</p>
<p>If the validation was added at the plan level, this field is blank.</p></td>
</tr>
<tr class="odd">
<td><p>Tag ID</p></td>
<td><p>Displays the name of the tag used to assign the Plan Task to the validation. If the validation is assigned directly to a plan or Plan Task (without using a tag), then this field is empty.</p></td>
</tr>
<tr class="even">
<td><p>Priority</p></td>
<td><p>Displays the order the validation runs if multiple validations are assigned to the plan.</p></td>
</tr>
<tr class="odd">
<td><p>Data Source ID</p></td>
<td><p>Displays the name of the data source that stores the validation.</p></td>
</tr>
<tr class="even">
<td><p>View/Procedure</p></td>
<td><p>Displays the validation name. The View or Procedure label on this field depends on the selection made in the VALIDATION TYPE list box on the <span style="font-style: italic;">Horizontal</span> View.</p></td>
</tr>
<tr class="odd">
<td><p>Work List Event ID</p></td>
<td><p>Displays the event that triggers the validation to run. Values are:</p>
<ul>
<li><strong>Finish</strong> – The validation runs when a user completes the a Plan Task for the plan on the Work List by clicking Next Action when the task has a status of In Progress.</li>
<li><strong>Start</strong> – The validation runs when a user starts work on a Plan Task in the plan on the Work List by clicking Next Action after the task has been created.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Active</p></td>
<td><p>If enabled, the validation is active. If disabled, the validation is inactive and will not run.</p></td>
</tr>
<tr class="odd">
<td><p>Validation Message</p></td>
<td><p>Displays a brief message that will display to the user if the validation fails. This message should contain information about why the validation failed, and how to correct the problem, if applicable.</p></td>
</tr>
<tr class="even">
<td><p>Description</p></td>
<td><p>Displays information about the SQL code used in the validation so that a user will not have to review the code to understand the validation.</p></td>
</tr>
</tbody>
</table>
