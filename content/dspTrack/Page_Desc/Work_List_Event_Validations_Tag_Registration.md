# Work List Event Validations - Tag Registration H

[Work List Event Validations - Tag Registration
V](#Work_List_Event_Validations_-_Tag_Registration_V)

<div class="use">

Use this page to [Configure Logic
Tags](../Use_Cases/Configure_Logic_Tags.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Track
    \></span>**Configuration \> Tag Type** in the *Navigation* pane.
2.  Click **Tags** for the Logic Tag Type.
3.  Click **Registrations** for the tag.
4.  Click **Validations**.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>TAG ID</p></td>
<td><p>Displays the name of the tag used to assign the task to the validation.</p>
<p><strong>NOTE</strong>: If the validation is assigned directly to a Plan Task or plan (without using a tag), then this field is empty.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the validation runs if multiple validations are assigned to the Plan Task.</p></td>
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
<li><strong>Finish</strong> - The validation runs when a user completes the selected task on the Work List by clicking Next Action when a task has a status of In Progress.</li>
<li><strong>Start</strong> - The validation runs when a user starts work on the selected task on the Work List by clicking Next Action when a task has a status of Ready.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If enabled, the validation is active. If disabled, the validation is inactive and will not run.</p></td>
</tr>
</tbody>
</table>

## <span id="Work_List_Event_Validations_-_Tag_Registration_V"></span>Work List Event Validations - Tag Registration V

[Work List Event Validations - Tag Registration H](#)

<div class="use">

Use this page to [Configure Logic
Tags](../Use_Cases/Configure_Logic_Tags.htm).

</div>

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Tag ID</p></td>
<td><p>Displays the name of the tag used to assign the task to the validation.</p>
<p><strong>NOTE</strong>: If the validation is assigned directly to a Plan Task or plan (without using a tag), then this field is empty.</p></td>
</tr>
<tr class="odd">
<td><p>Priority</p></td>
<td><p>Displays the order the validation runs if multiple validations are assigned to a Plan Task.</p></td>
</tr>
<tr class="even">
<td><p>Data Source ID</p></td>
<td><p>Displays the name of the data source that stores the validation.</p></td>
</tr>
<tr class="odd">
<td><p>View/Procedure</p></td>
<td><p>Displays the validation name. The label on this field depends on the Validation Type selected on the <span style="font-style: italic;">Horizontal</span> view.</p></td>
</tr>
<tr class="even">
<td><p>Work List Event ID</p></td>
<td><p>Displays the event that triggers the validation to run. Values are:</p>
<ul>
<li><strong>Finish</strong> - The validation runs when a user completes the selected task on the Work List by clicking Next Action when the task has a status of In Progress.</li>
<li><strong>Start</strong> - The validation runs when a user starts work on the selected task on the Work List by clicking Next Action when the task has a status of Ready.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Active</p></td>
<td><p>If enabled, the validation is active. If disabled, the validation is inactive and will not run.</p></td>
</tr>
<tr class="even">
<td><p>Validation Message</p></td>
<td><p>Displays a brief message that will display to the user if the validation fails. This message should contain information about why the validation failed, and how to correct the problem, if applicable.</p></td>
</tr>
<tr class="odd">
<td><p>Description</p></td>
<td><p>Displays information about the SQL code used in the validation so that a user will not have to review the code to understand the validation.</p></td>
</tr>
</tbody>
</table>
