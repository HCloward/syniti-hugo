+++
title = 'Work List Setup H'
solution = 'Platform'
+++

# Work List Setup H

[Work List Setup V](#Work_List_Setup_V)

<div class="use">

Use this page to [Add Work List
Items](../Use_Cases/Add_Work_List_Items_Overview).

</div>

To access this page, select **Track \> Configuration \> Work List**.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>ITEM NAME</p></td>
<td><p>Displays the name of the Work List Item or Plan Task.</p></td>
</tr>
<tr class="odd">
<td><p>STATUS</p></td>
<td><p>Displays the Plan Task’s or Work List Item’s status. Refer to <a href="Task_Status1">Task Status</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>PROJECT</p></td>
<td><p>Displays the name of the project containing the plan that contains the task. If the item is a Work List Item, this field is blank.</p></td>
</tr>
<tr class="odd">
<td><p>PLAN</p></td>
<td><p>Displays the name of the plan that contains the task. If the item is a Work List Item, this field is blank.</p></td>
</tr>
<tr class="even">
<td><p>PLANNED START DATE</p></td>
<td><p>Displays the planned start date for work on the item according to the project plan.</p></td>
</tr>
<tr class="odd">
<td><p>PLANNED FINISH DATE</p></td>
<td><p>Displays the planned finish date for work on the item according to the project plan.</p></td>
</tr>
<tr class="even">
<td><p>PAGE ID</p></td>
<td><p>Displays the name of the component and page that will open when the user clicks the PAGE ID link on the <span style="font-size: 11.0pt;">Work List</span>.</p></td>
</tr>
<tr class="odd">
<td><p>Keys</p></td>
<td><p>Click to open the <em><a href="Work_List_Binding_Criteria">Work List Binding Criteria</a></em> page to set a value for the key(s) of the page that will open when the user clicks the PAGE ID link on the <span style="font-size: 11.0pt;">Work List</span>.</p>
<p><strong>NOTE:</strong> The number that displays on the icon is the number of keys that have key values set on the Work List Binding Criteria page. Depending on the page selected in the PAGE ID list box on the Work List Setup page, the Work List Binding Criteria page may display a single key or multiple keys.</p></td>
</tr>
<tr class="even">
<td><p>Users</p></td>
<td><p>Click to open the <em><a href="Work_List_Item_User">Work List Item User</a></em> page to add users to and remove users from the item. Items assigned to a user display for that user on the <span style="font-size: 11.0pt;">Work List</span>.</p>
<p><strong>NOTE:</strong> User assignments for Plan Tasks cannot be changed here, and must be set on the <em><span style="font-size: 11.0pt;"><a href="Plan_Task_User"><span style="font-size: 11.0pt;">Plan Task User</span></a></span></em> page (Project &gt; Plans &gt; Tasks &gt; Users).</p></td>
</tr>
<tr class="odd">
<td><p>Uploads</p></td>
<td><p>Click to open the <em><a href="File_Upload_Work_List">File Upload Work List</a></em> page to view and upload files for the selected item.</p></td>
</tr>
<tr class="even">
<td><p>Rules</p></td>
<td><p>Click to open the <em><a href="Work_List_Event_Rule_Work_List_Setup"><em>Work List Event Rule<span style="font-size: 11.0pt;">– Work List Setup</span></em></a></em> page to add, edit and delete Work List Event rules for the selected item.</p>
<p><strong>NOTE:</strong> Work List Event Rules for Plan Tasks cannot be changed here, and must be set on the <em><span style="font-size: 11.0pt;">Work List Event Rule -</span>Plan Task</em> page (Project &gt; Plans &gt; Tasks &gt; Rules).</p></td>
</tr>
<tr class="odd">
<td><p>Validations</p></td>
<td><p>Click to open the <em><a href="Work_List_Event_Validations_Work_List_Setup_H"><em>Work List Event Validations– Work List Setup</em></a></em> page to add, edit and delete Work List Event validations for the selected item.</p>
<p><strong>NOTE:</strong> Work List Event Validations for Plan Tasks cannot be changed here, and must be set on the <em><span style="font-size: 11.0pt;">Work List Event Validation</span></em> - <em>Plan Task</em> page (Project &gt; Plans &gt; Tasks &gt; Validations).</p></td>
</tr>
</tbody>
</table>

## <span id="Work_List_Setup_V"></span>Work List Setup V

[Work List Setup H](Work_List_Setup_H)

<div class="use">

Use this page to [Add Work List
Items](../Use_Cases/Add_Work_List_Items_Overview).

</div>

Field

Description

Item Name

Displays the name of the Work List Item or Plan Task.

Item Description

Displays a brief description of the item.

Planned Start Date

Displays the planned start date for work on the item.

Planned Finish Date

Displays the planned finish date for work on the item.

**NOTE:** The PLANNED FINISH DATE must be later than the PLANNED START
DATE.

**NOTE:** If the Planned Finish Date is before the current date, this
item does not display on the Work List.

Audit Information

Actual Start Date

Displays the date work started on the item, when the item moved from
Ready status to In Progress status when a user clicked Next Action on
the Work List.

Started By

Displays the user ID of the user who started work on the item.

Actual Finish Date

Displays the date work finished on the item, when the item moved from In
Progress status to Completed status when a user clicked Next Action on
the Work List.

**NOTE:** If the Actual Finish Date is before the current date, this
item does not display on the Work List.

Finished By

Displays the user ID of the user who finished work on the item.

LinkToPage

Displays the name of the component and page that opens when the user
clicks the PAGE ID icon on the Work List.
