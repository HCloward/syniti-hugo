+++
title = 'Work List Event Validations - Work List Setup H'
solution = 'Platform'
+++

# Work List Event Validations - Work List Setup H

[Work List Event Validations - Work List Setup
V](#Work_List_Event_Validations_-_Work_List_Setup_V)

<div class="use">

Use this page to [Register Work List Event Validations for Work List
Items](../Use_Cases/Register_WorkList_Event_Valid_WorkList_Item).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Track \></span>
    **Configuration \> Work List** in the *Navigation* pane.
2.  Click **Validations** for a Work List Item.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>WORK LIST ITEM ID</p></td>
<td><p>Displays the name of Work List Item associated with the validation.</p>
<p><strong>NOTE</strong>: If the validation was added to plan or Plan Task, this field is blank.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the validation runs if multiple validations are assigned to the Work List item.</p></td>
</tr>
<tr class="even">
<td><p> DATA SOURCE ID</p></td>
<td><p>Displays the name of the data source that stores the validation.</p></td>
</tr>
<tr class="odd">
<td><p>VALIDATION TYPE</p></td>
<td><p>Displays whether the validation is a stored procedure or a view.</p></td>
</tr>
<tr class="even">
<td><p>WORK LIST EVENT ID</p></td>
<td><p>Displays the event that triggers the validation to run. Values are:</p>
<ul>
<li><strong>Finish</strong> – The validation runs when a user completes the Work List Item on the Work List by clicking Next Action when the item has a status of In Progress.</li>
<li><strong>Start</strong> – The validation runs when a user starts work on the Work List Item on the Work List by clicking Next Action when the item has a status of Ready.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>NAME</p></td>
<td><p>Displays the validation name.</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If enabled, the validation is active. If disabled, the validation is inactive and will not run.</p></td>
</tr>
</tbody>
</table>

## <span id="Work_List_Event_Validations_-_Work_List_Setup_V"></span>Work List Event Validations - Work List Setup V

[Work List Event Validations - Work List Setup H](#)

<div class="use">

Use this page to [Register Work List Event Validations for Work List
Items](../Use_Cases/Register_WorkList_Event_Valid_WorkList_Item).

</div>

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Work List Item ID</p></td>
<td><p>Displays the name of Work List Item associated with the validation.</p>
<p><strong>NOTE</strong>: If the validation was added to plan or Plan Task, this field is blank.</p></td>
</tr>
<tr class="odd">
<td><p>Priority</p></td>
<td><p>Displays the order the validation runs if multiple validations are assigned to the Work List item.</p></td>
</tr>
<tr class="even">
<td><p>Data Source ID</p></td>
<td><p>Displays the name of the data source that stores the validation.</p></td>
</tr>
<tr class="odd">
<td><p>View/Procedure</p></td>
<td><p>Displays the validation name.</p></td>
</tr>
<tr class="even">
<td><p>Work List Event ID</p></td>
<td><p>Displays the event that triggers the validation to run. Values are:</p>
<ul>
<li><strong>Finish</strong> – The validation runs when a user completes the Work List Item on the Work List by clicking Next Action when the item has a status of In Progress.</li>
<li><strong>Start</strong> – The validation runs when a user starts work on the Work List Item on the Work List by clicking Next Action when the item has a status of Ready.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Active</p></td>
<td><p>If enabled, the validation is active. If disabled, the validation is inactive and will not run.</p></td>
</tr>
<tr class="even">
<td><p>Validation Message</p></td>
<td><p>Displays a brief message that will display to the user if the validation fails for the Work List Item.</p></td>
</tr>
<tr class="odd">
<td><p>Description</p></td>
<td><p>Displays information about the SQL code used in the validation so that a user will not have to review the code to understand the validation.</p></td>
</tr>
</tbody>
</table>
