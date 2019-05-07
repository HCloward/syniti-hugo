+++
title = 'Task H'
solution = 'Data Quality'
+++

# Task H

[Task V](#Task_V)

<div class="use">

Use this page to [Add a Task](../Use_Cases/Add_a_Task.htm).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspConduct
    \></span><span style="font-weight: bold;">Design </span>in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Tasks</span> icon for a
    category.

**NOTE:** If a task was imported from IGC™, data that was entered in
IGC™ cannot be updated from within dspConduct™, and many of the fields
and icons associated with the record are not active for that task. Refer
to [Update Custom Attributes for Governance
Elements](../Use_Cases/Update_Custom_Attributes_for_Governance_Elements.htm)
for more information.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>From IGC</p></td>
<td><p>Displays to indicate that the task was created in IGC™.</p>
<p>This column displays after the IGC™ parameters are configured in Common on initial install. Refer to the <em>BackOffice Associates® Installation and Upgrade Manual</em> for more information.</p>
<p><strong>NOTE</strong>: Data entered in IGC™ cannot be updated from within dspConduct™.</p>
<p><strong>NOTE</strong>: Records that come from IGC™ cannot be deleted.</p></td>
</tr>
<tr class="odd">
<td><p>TASK ID</p></td>
<td><p>Displays the name of the task assigned to the role.</p>
<p><strong>NOTE:</strong> Tasks are limited to pages in the default WebApp. The default WebApp is set at the Category level. Refer to <a href="../Use_Cases/Create_a_Category.htm">Create a Category</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>TYPE</p></td>
<td><p>Displays the task type assigned to the task on the <span style="font-style: italic;"><a href="#">Task</a></span> page. Task types are:</p>
<ul>
<li><span style="font-weight: bold;">Application</span> – Identifies tasks that gather, enter or make changes to data using pages in the Content WebApp for preparation to send to the system(s) of record.</li>
<li><span style="font-weight: bold;">Display</span> – Identifies tasks that can be viewed but cannot be changed.</li>
</ul>
<p><strong>NOTE:</strong> A task can also be set to read only when it is added to a role. Refer to <a href="../Use_Cases/Add_a_Task_to_a_Role.htm">Add a Task to a Role</a> for more information.</p>
<ul>
<li><span style="font-weight: bold;">Review</span> – Identifies tasks that evaluate and review data, either approving or rejecting all changes made within the execution of a request.</li>
<li><span style="font-weight: bold;">Post</span> – Identifies tasks that post data to a target system, after the Application and Review roles have been completed.</li>
</ul>
<p>Task types are used in conjunction with role types to control which tasks can be assigned to a role. Refer to <a href="../Use_Cases/Role_Types_and_Task_Types.htm">Role Types and Task Types</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>COMMENT</p></td>
<td><p>Displays a user-entered comment.</p></td>
</tr>
<tr class="even">
<td><p>Variants</p></td>
<td><p>Click to open the <a href="Task_Variant.htm">Task Variant</a> page. Refer to <a href="../Use_Cases/Add_a_Variant_to_a_Task.htm">Add a Variant to a Task</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Pages</p></td>
<td><p>Click to open the <a href="Task_Page_H.htm">Task Page</a> page to view a list of all pages associated with the selected task, including page name, type, and the column used to access a page if applicable.</p></td>
</tr>
<tr class="even">
<td><p>Final Finish Tables</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Task_Final_Finish_Tables_H.htm">Task Final Finish Tables</a></span> page to add tables that are used during the Final Finish process for the task. dspConduct™ downloads the data posted by a dspConduct™ request to tables in a target database (usually dgSAP). The data downloads using a CranPort package or a Data Services job. Refer to <a href="../Use_Cases/Final_Finish_Process_for_a_Request_Overview.htm">Final Finish Process for a Request Overview</a> for more information.</p>
<p><strong>NOTE:</strong> The count on the icon represents the number of final finish tables that are registered for the selected task.</p></td>
</tr>
<tr class="odd">
<td><p>Where Used</p></td>
<td><p>Click to open the Where Used – Task page to view the scenarios and roles that use the task, including a count of active and inactive scenarios and roles.</p></td>
</tr>
</tbody>
</table>

## <span id="Task_V"></span>Task V

[Task H](#)

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Task ID</p></td>
<td><p>Displays the name of the task assigned to the role.</p>
<p><strong>NOTE:</strong> Tasks are limited to pages in the default WebApp. The default WebApp is set at the Category level. Refer to <a href="../Use_Cases/Create_a_Category.htm">Create a Category</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Type</p></td>
<td><p>Displays the task type assigned to the task on the <span style="font-style: italic;"><a href="#">Task</a></span> page. Task types are:</p>
<ul>
<li><span style="font-weight: bold;">Application</span> – Identifies tasks that gather, enter or make changes to data using pages in the Content WebApp for preparation to send to the system(s) of record.</li>
<li><span style="font-weight: bold;">Display</span> – Identifies tasks that can be viewed but cannot be changed.</li>
</ul>
<p><strong>NOTE:</strong> A task can also be set to read only when it is added to a role. Refer to <a href="../Use_Cases/Add_a_Task_to_a_Role.htm">Add a Task to a Role</a> for more information.</p>
<ul>
<li><span style="font-weight: bold;">Review</span> – Identifies tasks that evaluate and review data, either approving or rejecting all changes made within the execution of a request.</li>
<li><span style="font-weight: bold;">Post</span> – Identifies tasks that post data to a target system, after the application and review roles have been completed.</li>
</ul>
<p>Task types are used in conjunction with role types to control which tasks can be assigned to a role. Refer to <a href="../Use_Cases/Role_Types_and_Task_Types.htm">Role Types and Task Types</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Comment</p></td>
<td><p>Displays a user-entered comment.</p></td>
</tr>
<tr class="odd">
<td><p>Documentation</p></td>
<td><p>Click to open the <a href="Element_Documentation.htm">Element Documentation</a> page to upload supporting documents for the task that can be used or displayed within the request when it is executed.</p>
<p>The count on the icon represents the number of files uploaded for the task.</p>
<p>Refer to <a href="../Use_Cases/Upload_Documentation_at_the_Task_Level.htm">Upload Documentation at the Task Level</a> for more information.  </p></td>
</tr>
<tr class="even">
<td><p>Instructions</p></td>
<td><p>Displays user-entered instructions for the task.</p></td>
</tr>
<tr class="odd">
<td><p>Where Used</p></td>
<td><p>Click to open the Where Used – Task page to view the scenarios and roles that use the task, including a count of active and inactive scenarios and roles.</p></td>
</tr>
</tbody>
</table>
