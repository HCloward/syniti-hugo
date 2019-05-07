+++
title = ''
solution = 'Master Data Management'
+++

# <span id="Request_Role_H"></span>Request Role H

[Request Role V](#Request_Role_V)

<div class="use">

Use this page to:

  - [View a Request’s Roles](../Use_Cases/View_a_Requests_Roles.htm)
  - [Validate a Role](../Use_Cases/Validate_a_Role.htm)

</div>

To access this page:

1.  Click **dspConduct \>Requests** in the *Navigation* pane.
2.  Click the **Roles** icon for a request.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Validate</p></td>
<td><p>Click to validate the selected role.</p>
<p>For each of the pages (including child pages) corresponding to the tasks for the request role, the process executes the validation views that have been registered to the pages. Any errors, warnings, or messages that result are displayed in a popup window on the page.</p>
<p><strong>NOTE:</strong> If a role has the Auto Extend Display option set on the <a href="Role_H_dspConduct.htm">Role</a> page’s Vertical View, this role displays as read only for all users assigned to roles in the Category. In other words, if a user is not assigned to a role, but the Auto Extend Display option is enabled for a role, the user can view (but not update) the role for the request regardless of whether the user is assigned to the role.</p>
<p>Refer to <a href="../Use_Cases/Validate_a_Role.htm">Validate a Role</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>ROLE ID</p></td>
<td><p>Displays the name of the role assigned to the request.</p>
<p>Refer to <a href="../Use_Cases/Add_a_Role.htm">Add a Role</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>DEPENDENCIES COMPLETE</p></td>
<td><p>If checked, all dependent roles for the selected role are finished.</p>
<p>Refer to <a href="../Use_Cases/Role_Dependencies.htm">Role Dependencies Overview</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>FINISHED ON</p></td>
<td><p>Displays the date and time when the role was finished.</p>
<p>Refer to <a href="../Use_Cases/Finish_a_Role_with_the_Application_Role_Type.htm">Finish a Role for the Application Role Type</a> and  <a href="../Use_Cases/Approve_a_Request.htm">Approve a Request</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>FINISHED BY</p></td>
<td><p>Displays the User ID of the individual who finished the role.</p>
<p>Refer to <a href="../Use_Cases/Finish_a_Role_with_the_Application_Role_Type.htm">Finish a Role for the Application Role Type</a> and <a href="../Use_Cases/Approve_a_Request.htm">Approve a Request</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>TASKS</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Request_Role_Task.htm">Request Role Task</a></span>page to view the tasks configured in the Content WebApp that are associated with the selected role ID.</p>
<p>The icon is active even if the tasks assigned to the role are not. Refer to <a href="../Use_Cases/Add_a_Task_to_a_Role.htm">Add a Task to a Role</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>FINISH</p></td>
<td><p>Click to finish (for roles with a type of Application or Post) or approve (for roles with a type of Review).</p>
<p>For roles other than the Post role, validations are automatically run. If there are validation errors, the process stops and subsequent rules are not executed. The Role Processor must fix the errors on the page before finishing the request. If no errors are encountered the stored procedures and other plugins are run to perform the Finish event.</p>
<p>When the role is finished, users assigned to the next role in the process are notified that their role is ready to be processed.</p>
<p><strong>NOTE:</strong> If a role has the Auto Extend Display option set on the <em><a href="Role_H_dspConduct.htm">Role</a></em> page’s <em>Vertical</em> View, this role displays as read only for all users assigned to roles in the Category. In other words, if a user is not assigned to a role, but the Auto Extend Display option is enabled for a role, the user can view (but not update) the role for the request regardless of whether the user is assigned to the role.</p>
<p><strong>NOTE:</strong> This button is disabled when the role is finished. If the role is reset, the button is active.</p>
<p>Refer to <a href="../Use_Cases/Finish_a_Role_with_the_Application_Role_Type.htm">Finish a Role for the Application Role Type</a> and <a href="../Use_Cases/Approve_a_Request.htm">Approve a Request</a>  for more information.</p></td>
</tr>
<tr class="odd">
<td><p>RESET</p></td>
<td><p>Click to reset (for roles with a type of Application or Post) or Reject (for roles with a type of Review) the role. This action indicates that the data is incorrect and the role is not ready to be finished. Users assigned to this role are notified via workflow email that their role has been reset or rejected.</p>
<p><strong>NOTE:</strong> If a role has the Auto Extend Display option set on the <a href="Role_H_dspConduct.htm">Role</a> page’s Vertical View, this role displays as read only for all users assigned to roles in the Category. In other words, if a user is not assigned to a role, but the Auto Extend Display option is enabled for a role, the user can view (but not update) the role for the request regardless of whether the user is assigned to the role.</p>
<p>Refer to <a href="../Use_Cases/Reset_a_Role.htm">Reset a Role</a> for more information.</p></td>
</tr>
</tbody>
</table>

## <span id="Request_Role_V"></span>Request Role V

[Request Role H](#Request_Role_H)

Field

Description

ROLE ID

Displays the name of the role assigned to the request.

Refer to [Add a Role](../Use_Cases/Add_a_Role.htm) for more information.

Validated On

Displays the date and time the request role was validated (as in, when a
user clicked the Validate icon in the Page toolbar on the
<span style="font-style: italic;">Horizontal</span> View).

Validated By

Displays the user ID of the user who validated the selected request
role.

Workflowed On

Displays the date and time a workflow related to this request role was
sent to the users assigned to the role.

**NOTE:** Workflow messages must be enabled for the role. Refer to
[Enable or Disable Messages for a
Role](../Use_Cases/Enable_or_Disable_Messages_for_a_Role.htm) for more
information.

Workflowed By

Displays the user ID of the user whose action on the selected role
resulted in a workflow email. This email is sent to the next assigned
role in the workflow.

**NOTE:** Workflow messages must be enabled for the role. Refer to
[Enable or Disable Messages for a
Role](../Use_Cases/Enable_or_Disable_Messages_for_a_Role.htm) for more
information.

Finish Download

**NOTE:** This section only displays for the Post role after a request
has been posted and Final Finish has executed.

Finish Download Message

Click to open the <span style="font-style: italic;">[Finish Download
Messages](../Use_Cases/Finish_Download_Messages.htm)</span> page to view
details about the posting during the Final Finish process.
