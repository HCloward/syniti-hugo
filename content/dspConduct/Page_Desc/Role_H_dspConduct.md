+++
title = 'Role H'
solution = 'Master Data Management'
+++

# Role H

[Role V](#Role_V)

<div class="use">

Use this page to [Add a Role](../Use_Cases/Add_a_Role).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspConduct
    \></span><span style="font-weight: bold;">Design</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    category.

**NOTE:** If a role was imported from IGC™, data that was entered in
IGC™ cannot be updated from within dspConduct™, and many of the fields
and icons associated with the record are not active for that role. Refer
to [Update Custom Attributes for Governance
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
<td><p>Displays to indicate that the role was created in IGC™.</p>
<p>This column displays after the IGC™ parameters are configured in Common on initial install. Refer to the <em>BackOffice Associates® Installation and Upgrade Manual</em> for more information.</p>
<p><strong>NOTE</strong>: Data entered in IGC™ cannot be updated from within dspConduct™.</p>
<p><strong>NOTE</strong>: Records that come from IGC™ cannot be deleted.</p></td>
</tr>
<tr class="odd">
<td><p>NAME</p></td>
<td><p>Displays the role name.</p>
<p>A role is a collection of tasks performed to support scenarios and business processes.</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a brief description of the role.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the role displays on the <span style="font-style: italic;">Roles</span> page.</p></td>
</tr>
<tr class="even">
<td><p>Tasks</p></td>
<td><p>Click to open the <a href="Role_Task">Role (Tasks)</a> page to add tasks to the role.</p>
<p>A task is a web page added to the Content WebApp at a client’s site.</p>
<p>Refer to <a href="../Use_Cases/Add_a_Task">Add a Task</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Dependencies</p></td>
<td><p>Click to open the <a href="Role_Dependencies">Role (Dependencies)</a> page to add a dependent role to the selected role. Refer to <a href="../Use_Cases/Role_Dependencies#Add_Dependencies_to_Roles">Add Dependencies to Roles</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Conflicts</p></td>
<td><p>Click to open the <a href="Role_Conflicts">Role (Conflicts)</a> page to add roles that can only be executed once per user in the scenario.</p>
<p>Refer to <a href="../Use_Cases/Add_a_Conflict_to_a_Role">Add a Conflict to a Role</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Where Used</p></td>
<td><p>Click to open the <span style="font-style: italic;">Where Used – Role</span> page to view the tasks assigned to the role and the scenarios that use the role. A count of active and inactive tasks and scenarios is also provided.</p>
<p><strong>NOTE:</strong> If any of the scenarios or business processes that the role is used in within a category are active, the role is considered active.</p></td>
</tr>
<tr class="even">
<td><p>Role Report</p></td>
<td><p>Click to open the <span style="font-style: italic;">Element Report Frame</span> page that displays basic information about the role; the role’s work days, hours and minutes; role dependencies; tasks to which the role is assigned; and positions that include the role.</p></td>
</tr>
</tbody>
</table>

## <span id="Role_V"></span>Role V

[Role H](Role_H_dspConduct)

<div class="use">

Use this page to [Configure the Post Later Feature at the Role
Level](../Use_Cases/Configure_the_Post_Later_Feature_at_the_Role_Level).

</div>

This page contains the following tabs:

  - [General](#General)
  - [Copy Options](#Copy_Options)

### <span id="General"></span>General

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Name</p></td>
<td><p>Displays the role name.</p>
<p>A role is a collection of tasks performed to support scenarios and business processes.</p></td>
</tr>
<tr class="odd">
<td><p>Description</p></td>
<td><p>Displays a brief description of the role.</p></td>
</tr>
<tr class="even">
<td><p>Owner</p></td>
<td><p>Displays the role owner.</p></td>
</tr>
<tr class="odd">
<td><p>Role Type</p></td>
<td><p>Displays the role type.</p>
<p>A role’s role type determines which actions a user assigned to that role can perform.</p>
<p>Role types are:</p>
<ul>
<li><span style="font-weight: bold;">Application</span> – Gathers, enters or makes changes to data using pages in the Content WebApp for preparation to send to the system(s) of record.</li>
<li><span style="font-weight: bold;">Display</span> – Views data but is unable to make changes. Users assigned to a role with a Display role type are not active participants in the process.</li>
<li><span style="font-weight: bold;">Review</span> – Evaluates and reviews data, either approving or rejecting all changes made within the execution of a request. Data can be viewed but not modified. A role with this role type can also review the tasks of their dependent application roles within a scenario.</li>
<li><span style="font-weight: bold;">Post</span> – Posts data to a target system after the roles with Application and Review role types have been completed.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Send Workflow</p></td>
<td><p>If enabled, the users assigned to the role receive a message during the request workflow depending on the user’s assigned role type. Refer to <a href="../Use_Cases/Enable_or_Disable_Messages_for_a_Role">Enable or Disable Messages for a Role</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Auto Extend Display</p></td>
<td><p>If enabled, the tasks within the role display as read only to all other users within the scenario not assigned to this role.</p></td>
</tr>
<tr class="even">
<td><p>User Response Required on Warnings</p></td>
<td><p>If enabled, after a user clicks Finish for the role, any validation failures require a user response to continue the process.</p>
<p>The options available to the user depend on the highest level of validation failure.</p>
<p>If the validation fails with a message, the user acknowledges the message by clicking the OK button to proceed.</p>
<p>If the validation fails with a warning, the user is presented with the options to allow the process to continue or to stop the process.</p>
<p>If the validation fails with an error, the user acknowledges the error and the process stops.</p>
<p><strong>NOTE</strong>: If this check box is disabled, if the validation fails with a warning, the user acknowledges the message by clicking the OK button to proceed.</p>
<p>This setting can be overridden at the scenario role level.</p></td>
</tr>
<tr class="odd">
<td><p>Work Days</p></td>
<td><p>Displays the number of days that all of the tasks in this role must be executed to meet the SLA. Refer to <a href="../Config/Set_Up_SLA_Notifications">Set up SLA notifications in dspConduct™</a> for more information.</p>
<p><strong>NOTE</strong>: If the role has been imported from IGC™, and this value has been updated in IGC™, that value overwrites the value in dspConduct™.</p></td>
</tr>
<tr class="even">
<td><p>Work Hours</p></td>
<td><p>Displays the number of hours that all of the tasks in this role must be executed to meet the SLA. Refer to <a href="../Config/Set_Up_SLA_Notifications">Set up SLA notifications in dspConduct™</a> for more information.</p>
<p><strong>NOTE</strong>: If the role has been imported from IGC™, and this value has been updated in IGC™, that value overwrites the value in dspConduct™.</p></td>
</tr>
<tr class="odd">
<td><p>Work Minutes</p></td>
<td><p>Displays the number of minutes that all of the<span> </span>tasks in this role must be executed to meet the SLA. Refer to <a href="../Config/Set_Up_SLA_Notifications">Set up SLA notifications in dspConduct™</a> for more information.</p>
<p><strong>NOTE</strong>: If the role has been imported from IGC™, and this value has been updated in IGC™, that value overwrites the value in dspConduct™.</p></td>
</tr>
<tr class="even">
<td><p>Scheduled Post Allowed</p></td>
<td><p>If enabled, a scenario that uses this role allows a user assigned to the Post role to schedule a post for a later time. Use this check box to:</p>
<ul>
<li>Set the default setting for new roles for a Post role added in the future.</li>
<li>Update this setting for all scenario &gt; role combinations that use this role.  </li>
</ul>
<p>This check box only displays for roles with a Role Type of Post.</p>
<p>After updating this check box, a message displays. If the user clicks OK, the update cascades through all scenario &gt; role combinations that use this role. If the user clicks Cancel, the selected setting (enabled or disabled) is retained as the default setting when roles with a Post role type are added in the future. However, the setting does not cascade through all scenario &gt; role combinations that use that role.</p>
<p>The setting can be overwritten for a specific scenario &gt; role combination, and it is at this level that access to the Post Later feature is controlled. Refer to <a href="../Use_Cases/Configure_the_Post_Later_Feature_at_the_Scenario_Role_Level">Configure the Post Later Feature at the Scenario Role Level</a>, <a href="../Use_Cases/Configure_the_Post_Later_Feature_at_the_Role_Level">Configure the Post Later Feature at the Role Level,</a> and <a href="../Use_Cases/Post_a_Request#Schedule_a_Post_for_a_Specified_Date_and_Time">Schedule a Post for a Specified Date and Time</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Documentation</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Element_Documentation">Element Documentation</a> page</span>  to upload documentation for this role, which may include additional instructions for the role, or a document that can be uploaded and exposed during execution of the role.</p>
<p>Refer to <a href="../Use_Cases/Upload_Documentation_at_the_Role_Level">Upload Documentation at the Role Level</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Where Used</p></td>
<td><p>Click to open the <span style="font-style: italic;">Where Used – Role</span> page to view the tasks assigned to the role and the scenarios that use the role. A count of active and inactive tasks and scenarios is also provided.</p></td>
</tr>
<tr class="odd">
<td><p>Role Report</p></td>
<td><p>Click to open a report displaying basic information about the role; the role’s work days, hours and minutes; role dependencies; tasks to which the role is assigned; and positions that include the role.</p></td>
</tr>
<tr class="even">
<td><p>Comment</p></td>
<td><p>Displays a user-entered comment about the role.</p></td>
</tr>
</tbody>
</table>

### <span id="Copy_Options"></span>Copy Options

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
<td><p>New Role Name</p></td>
<td><p>Displays the name of the new role created as a result of copying the selected role.</p>
<p>The new role name must be unique.</p></td>
</tr>
<tr class="odd">
<td><p>Copy</p></td>
<td><p>Click to create a copy of the selected role.</p></td>
</tr>
</tbody>
</table>
