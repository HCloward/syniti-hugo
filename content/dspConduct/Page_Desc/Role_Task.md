+++
title = 'Role (Tasks)'
solution = 'Master Data Management'
+++

# Role (Tasks)

<div class="use">

Use this page to [Add a Task to a
Role](../Use_Cases/Add_a_Task_to_a_Role).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspConduct \> Design
    </span>in the <span style="font-style: italic;">Navigation</span>
    pane.
2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    category.
3.  Click the <span style="font-weight: bold;">Tasks</span> icon for a
    role.

**NOTE:** If a task was assigned to a role and imported from IGC™, data
that was entered in IGC™ cannot be updated from within dspConduct™, and
many of the fields and icons associated with the record are not active
for that role task. Refer to [Update Custom Attributes for Governance
Elements](../Use_Cases/Update_Custom_Attributes_for_Governance_Elements)
for more information.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>From IGC</p></td>
<td><p>Displays to indicate that the task was assigned to the role in IGC™.</p>
<p>This column displays after the IGC™ parameters are configured in Common on initial install. Refer to the <em>BackOffice Associates® Installation and Upgrade Manual</em> for more information.</p>
<p><strong>NOTE</strong>: Data entered in IGC™ cannot be updated from within dspConduct™.</p>
<p><strong>NOTE</strong>: Records that come from IGC™ cannot be deleted.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the order a task displays on the <span style="font-style: italic;">Role (Task)</span> page.</p></td>
</tr>
<tr class="even">
<td><p>TASK ID</p></td>
<td><p>Displays the name of the task assigned to the role.</p>
<p><strong>NOTE:</strong> The pages available for a task are those pages in the Content WebApp set at the Category level in the Default Web App ID field on the <a href="Category_H">Category</a> page.</p>
<p><strong>NOTE:</strong> These tasks were added on the <span style="font-style: italic;"><a href="Task_H">Task</a></span> page. To add a task, click the + icon in the list box. Refer to <a href="../Use_Cases/Add_a_Task">Add a Task</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>TYPE</p></td>
<td><p>Displays the task type assigned to the task on the <span style="font-style: italic;">Task</span> page. Task types are:</p>
<ul>
<li><span style="font-weight: bold;">Application</span> – Identifies tasks that gather, enters or makes changes to data using pages in the Content WebApp for preparation to send to the system(s) of record.</li>
</ul>
<p><strong>NOTE:</strong> A task can be set to read only for a role.  Users can view the task’s data but cannot make changes to the data</p>
<ul>
<li><span style="font-weight: bold;">Display</span> – Identifies tasks that can be viewed but cannot be changed.</li>
<li><span style="font-weight: bold;">Review</span> – Identifies tasks that evaluate and review data, either approving or rejecting all changes made within the execution of a request.</li>
<li><span style="font-weight: bold;">Post</span> – Identifies tasks that post data to a target system, after the application and review roles have been completed.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>READ ONLY</p></td>
<td><p>If enabled, the task’s associated web page displays as read only for a role. Users can view the task’s data but cannot make changes to the data.</p>
<p>If disabled, the task can be updated.</p></td>
</tr>
<tr class="odd">
<td><p>Assigned Scenarios</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Scenario_Role_Task_H">Scenario Role Task</a></span> page to view details about the selected role and task, including the columns available on the web page associated with the task.</p></td>
</tr>
</tbody>
</table>
