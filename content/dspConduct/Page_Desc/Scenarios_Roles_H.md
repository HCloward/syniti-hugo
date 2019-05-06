# Scenarios (Roles) H

[Scenarios (Roles) V](#Scenarios__Roles__V)

<div class="use">

Use this page to [Add a Role to a
Scenario](../Use_Cases/Add_a_Role_to_a_Scenario.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspConduct
    \></span>**Design<span style="font-weight: normal;"> in the
    </span><span style="font-weight: normal;font-style: italic;">Navigation</span><span style="font-weight: normal;">
    pane.</span>**
2.  Click the **Scenarios** icon.
3.  Click the **Roles** icon.

**NOTE:** If a role was assigned to a scenario and imported from IGC™,
data that was entered in IGC™ cannot be updated from within dspConduct™,
and many of the fields and icons associated with the record are not
active for that scenario role. Refer to [Update Custom Attributes for
Governance
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
<td><p>Displays to indicate that the role was assigned to the scenario in IGC™.</p>
<p>This column displays after the IGC™ parameters are configured in Common on initial install. Refer to the <em>BackOffice Associates® Installation and Upgrade Manual</em> for more information.</p>
<p><strong>NOTE</strong>: Data entered in IG™C cannot be updated from within dspConduct™.</p>
<p><strong>NOTE</strong>: Records that come from IGC™ cannot be deleted.</p></td>
</tr>
<tr class="odd">
<td><p>ROLE</p></td>
<td><p>Displays the role ID assigned on the <em>Role</em> page.</p>
<p>When adding roles to a scenario, if a role is not in the list box, the user can click the <strong>Click to add a new item</strong> link to open the <em>Role</em> page in another browser tab. Refer to <a href="../Use_Cases/Add_a_Role.htm">Add a Role in dspConduct™</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>ROLE ID</p></td>
<td><p>Displays the role ID assigned on the <em><a href="Role_H_dspConduct.htm">Role</a></em> page.</p>
<p>When adding roles to a scenario, if a role is not in the list box, the user can click the <strong>Click to add a new item</strong> link to open the <em>Role</em> page in another browser tab. Refer to <a href="../Use_Cases/Add_a_Role.htm">Add a Role in dspConduct™</a> for more information.</p>
<p><strong>NOTE</strong>: This field displays roles that have tasks assigned or roles that were imported form IGC™. Roles added in dspConduct™ without tasks do not display.</p></td>
</tr>
<tr class="odd">
<td><p>WORK DAYS</p></td>
<td><p>Displays the number of days estimated to complete the tasks assigned to the role.</p>
<p><strong>NOTE:</strong> Leave blank to default to the values set up on <em>Roles</em> page’s <em>Vertical</em> View. Refer to <a href="../Config/Set_Up_SLA_Notifications.htm">Set up SLA notifications in dspConduct™</a> for more information.</p>
<p><strong>NOTE</strong>: When a role is imported from IGC™ and this field is blank in dspConduct™, the value entered in IGC™ is used. If this field already contains a value in dspConduct™, this value is not updated.</p></td>
</tr>
<tr class="even">
<td><p>WORK HOURS</p></td>
<td><p>Displays the number of hours estimated to complete the tasks assigned to the role.</p>
<p><strong>NOTE:</strong> Leave blank to default to the values set up on <em>Roles</em> page’s <em>Vertical</em> View. Refer to <a href="../Config/Set_Up_SLA_Notifications.htm">Set up SLA notifications in dspConduct™</a> for more information.</p>
<p><strong>NOTE</strong>: When a role is imported from IGC™ and this field is blank in dspConduct™, the value entered in IGC™ is used. If this field already contains a value in dspConduct™, this value is not updated.</p></td>
</tr>
<tr class="odd">
<td><p>WORK MINUTES</p></td>
<td><p>Displays the number of minutes estimated to complete the tasks assigned to the role.</p>
<p><strong>NOTE</strong>: Leave blank to default to the values set up on <em>Roles</em> page’s <em>Vertical</em> View. Refer to <a href="../Config/Set_Up_SLA_Notifications.htm">Set up SLA notifications in dspConduct™</a> for more information.</p>
<p><strong>NOTE</strong>: When a role is imported from IGC™ and this field is blank in dspConduct™, the value entered in IGC™ is used. If this field already contains a value in dspConduct™, this value is not updated.</p></td>
</tr>
<tr class="even">
<td><p>Events</p></td>
<td><p>Click to open the <a href="Scenario_Role_Event.htm">Scenario Role Event</a> page to add a custom business rule to an even for the selected role.</p>
<p>Refer to <a href="../Use_Cases/Add_Custom_Business_Rules.htm">Add Custom Business Rules</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Tasks</p></td>
<td><p>Click to open the <em><a href="Scenario_Role_Task_H.htm">Scenario Role Task</a></em> page.</p></td>
</tr>
</tbody>
</table>

## <span id="Scenarios__Roles__V"></span>Scenarios (Roles) V

[Scenarios (Roles) H](Scenarios_Roles_H.htm)

<div class="use">

Use this page to [Configure the Post Later Feature at the Scenario -
Role
Level](../Use_Cases/Configure_the_Post_Later_Feature_at_the_Scenario_Role_Level.htm).

</div>

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Role</p></td>
<td><p>Displays the role ID assigned on the <em>Role</em> page.</p>
<p>When adding roles to a scenario, if a role is not in the list box, the user can click the <strong>Click to add a new item</strong> link to open the <em>Role</em> page in another browser tab. Refer to <a href="../Use_Cases/Add_a_Role.htm">Add a Role in dspConduct™</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Auto Post Role</p></td>
<td><p>Click to enable the role as an auto post role within the scenario.</p>
<p><strong>NOTE:</strong> This option only displays for roles of type Post. If this option is enabled, then once the request data dependencies have been completed, posting is automatically initiated. A user is not required to click the Post button to initiate the posting. Refer to <a href="../Use_Cases/Post_a_Request.htm#Auto_Post_a_Request">Auto Post a Request</a>  for more information.</p>
<p><strong>NOTE:</strong> The Auto Post Role feature can only be used if default credentials are set for all connections used by the scenario's Integrate processes. Refer to <a href="../Use_Cases/Add_an_Integrate_Process_to_a_Scenario.htm">Add a Process to a Scenario</a> and <a href="../../../Platform/Common/Use_Cases/Add_Default_User_Credentials_to_a_Connection.htm">Add Default User Credentials to a Connection</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Auto Finish Role</p></td>
<td><p>Click to enable the role as an auto finish role within the scenario.</p></td>
</tr>
<tr class="odd">
<td><p>User Response Required on Warnings</p></td>
<td><p>If enabled, after a user clicks Finish for the role, any validation failures require a user response to continue the process.</p>
<p>The options available to the user depend on the highest level of validation failure.</p>
<ul>
<li>If the validation fails with a message, the user acknowledges the message by clicking the OK button to proceed.</li>
<li>If the validation fails with a warning, the user is presented with the options to allow the process to continue or to stop the process.</li>
<li>If the validation fails with an error, the user acknowledges the error and the process stops.</li>
</ul>
<p><strong>NOTE</strong>: If this check box is disabled, if the validation fails with a warning, the user acknowledges the message by clicking the OK button to proceed.</p>
<p>The default value for this setting is set at the Role level.</p></td>
</tr>
<tr class="even">
<td><p>Scheduled Post Allowed</p></td>
<td><p>If enabled, a user assigned to this scenario &gt; role combination can schedule a posting to run at a later time. The Post Later options display on the <span style="font-style: italic;"><a href="Request_Group_Post.htm">Request Group Post</a></span> page. If disabled, the Post Later options do not display on the <span style="font-style: italic;">Request Group Post</span> page.</p>
<p>The setting can also be configured for all scenario &gt; role combinations on the <span style="font-style: italic;"><a href="Role_H_dspConduct.htm">Role</a></span> page. </p>
<p>Refer to <a href="../Use_Cases/Configure_the_Post_Later_Feature_at_the_Scenario_Role_Level.htm">Configure the Post Later Feature at the Scenario Role Level</a>, <a href="../Use_Cases/Configure_the_Post_Later_Feature_at_the_Role_Level.htm">Configure the Post Later Feature at the Role Level,</a> and <a href="../Use_Cases/Post_a_Request.htm#Schedule_a_Post_for_a_Specified_Date_and_Time">Schedule a Post for a Specified Date and Time</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Allow Update For Extend Scenarios</p></td>
<td><p>Click to enable to allow the role to update system data within a task that already exists in the target.</p>
<p><strong>NOTE:</strong> This option is only available for roles of type Application assigned to scenarios of type BusinessExtend or OrganizationalExtend.</p></td>
</tr>
<tr class="even">
<td><p>Post Workflow Notifications</p></td>
<td><p>Click to open the<span style="font-style: italic;"> <a href="Post_Workflow_Notification.htm">Post Workflow Notification</a></span> page to add external users and register platform users who receive workflow notifications when a post succeeds or fails.</p>
<p>The count on the icon represents the number of users who receive these notifications.</p></td>
</tr>
<tr class="odd">
<td><p>Documentation</p></td>
<td><p>Click to open the <em><a href="Element_Documentation.htm">Element Documentation</a></em> page to upload or download documentation regarding the scenario role.</p>
<p>Refer to <a href="../Use_Cases/Upload_Documentation_at_the_Scenario_Role_Level.htm">Upload Documentation at the Scenario Role Level</a> more information.</p></td>
</tr>
</tbody>
</table>
