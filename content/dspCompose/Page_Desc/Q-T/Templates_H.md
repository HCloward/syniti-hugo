+++
title = 'Templates H'
solution = 'Data Quality'
+++

# Templates H

[Templates V](#Templates_V_All_Tabs)

<div class="use">

Use this page to

  - [Create a Template from the Templates
    Page](../Use_Cases/Create_a_Template_from_the_Templates_Page.htm)
  - [Create a Template that Uses the Custom Pages in
    dspCompose™](../Use_Cases/Create_a_Template_that_uses_the_Custom_Pages.htm)

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspCompose \>
    Team</span> on the *Navigation *pane.
2.  Click the **Templates** icon for a team.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>TEMPLATE NAME</p></td>
<td><p>Displays the template name. A template is a way to manage data in the form of a particular process, for example, to create a new BOM or to change a material.</p></td>
</tr>
<tr class="odd">
<td><p>TRANSACTION CODE</p></td>
<td><p>Displays target ERP system transaction used in the template recording. A transaction code is not needed if creating a custom template (as in, if the Type is set to Custom Setup).</p></td>
</tr>
<tr class="even">
<td><p>TYPE</p></td>
<td><p>Displays the posting type for the template.</p>
<p>Values are:</p>
<ul>
<li><strong>BDC Script –</strong> The  template is based on the results of a Batch Data Communication (BDC) script recorded in dspCompose</li>
<li><strong>GUI Script –</strong> The template is based on the results of a GUI script recorded using the SAP Logon pad</li>
<li><strong>Custom Setup –</strong> The template is custom and is not created using a recording</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>ACTIVE</p></td>
<td><p>If enabled, the template is active. A template must be active to use for requests.</p></td>
</tr>
<tr class="even">
<td><p>ACTIVATE/DEACTIVATE</p></td>
<td><p>Click to activate or deactivate the template. A template can be activated if:</p>
<ul>
<li>It has not been generated.</li>
<li>Each role assigned to the template is not dependent on another role assigned to the template, or does not have a dependency on another role assigned to the template.</li>
</ul>
<p>A template cannot be deactivated if active requests exist for the template. A request is considered Active when it is in an <span id="dspCompose Request Status" class="popUpLink">active request status</span>.</p></td>
</tr>
<tr class="odd">
<td><p>Requests</p></td>
<td><p>Click to open the <em><a href="Request_H.htm">Request</a></em> page to add, edit and process requests based on the template. This icon is only active if requests that use this template exist.</p></td>
</tr>
<tr class="even">
<td><p>Roles</p></td>
<td><p>Click to open the <em><a href="Template_Role_H.htm">Template (Role)</a></em> page to add, edit and delete roles assigned to the template.</p>
<p><strong>NOTE:</strong> The count on this icon indicates the number of roles assigned to the template. Global roles with the Auto Copy option set on the <span style="font-style: italic;"><a href="Roles_H.htm">Roles</a></span> page are automatically added to a template when it is created. Refer to <a href="../Config/Add_a_Global_Role.htm">Add a Global Role</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Org Units</p></td>
<td><p>Click to open the <em><a href="Template_Org_Units_H.htm">Template (Org Units)</a></em> page to add, edit and delete Org Units assigned to the template. Org units are optional for templates.</p>
<p><strong>NOTE:</strong> The count on this icon indicates the number of Org Units assigned to the template. Refer to <a href="../Use_Cases/Set_up_Org_Units.htm#Add_Org_Units_to_a_Template">Add Org Units to a Template</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Users</p></td>
<td><p>Click to open the <em><a href="Template_Users_H.htm">Template (Users)</a></em>page to add, edit or delete users who have been granted access to the template. The user who created the template is automatically assigned to the template and to all the roles.</p>
<p><strong>NOTE:</strong> The count on this icon indicates the number of users granted access to the template. The user who created the template is automatically assigned to the template and to all the template’s roles.</p></td>
</tr>
<tr class="odd">
<td><p>External Request Scenarios</p></td>
<td><p>Click to open the <em><a href="Template_External_Request_Scenario.htm">Template (External Request Scenario)</a></em> page to add, edit and delete external request scenarios, including external request scenarios that create Excel-initiated requests.</p>
<p><strong>NOTE:</strong> The number on the icon represents the number of external request scenarios that exist for the template.</p></td>
</tr>
<tr class="even">
<td><p>ISA External Request Scenarios</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="../../ISA/Page_Desc/Template_ISA_External_Request_Scenario_H.htm">Template (ISA External Request Scenario)</a></span> page to add, edit or delete an external request scenario that uses data from an ISA report as the basis for a request.</p>
<p><strong>NOTE:</strong> This icon does not display if the ISA is not installed and licensed.</p></td>
</tr>
</tbody>
</table>

## <span id="Templates_V_All_Tabs"></span>Templates V All Tabs

[Templates H](Templates_H.htm)

This page contains the following tabs:

  - [General tab](#General_Tab4)
  - [Configuration tab](#Configuration_Tab)
  - [Advanced tab](#Advanced_Tab)

## <span id="General_Tab4"></span>General tab

Field

Description

Activate/Deactivate

Click to activate or deactivate the template. A template can beactivated
if:

  - It has not been generated.
  - Each role assigned to the template is not dependent on another role
    assigned to the template, or does not have a dependency on another
    role assigned to the template.

A template cannot be deactivated if active requests exist for the
template. A request is considered Active when it is in an
<span id="dspCompose Request Status" class="popUpLink">active request
status</span>.

Requests

Click to open the *[Request](Request_H.htm)* page to add, edit and
process requests based on the template. This icon is only active if
requests that use this template exist.

Details

Template Name

Displays the template name. A template is a way to manage data in the
form of a particular process, for example, to create a new BOM or to
change a material.

Transaction Code

Displays target ERP system transaction used in the template recording. A
transaction code is not needed if creating a custom template (as in, if
the Type is set to Custom Setup).

Type

Displays the posting type for the template.

Values are:

  - **BDC Script –** The  template is based on the results of a Batch
    Data Communication (BDC) script recorded in dspCompose
  - **GUI Script –** The template is based on the results of a GUI
    script recorded using the SAP Logon pad
  - **Custom Setup –** The template is custom and is not created using a
    recording

Connection

Connection ID

Displays the connection to the target system that was set for the user
credentials for this template.

The connection is set on the *[User
Credentials](../../../Platform/Common/Page_Desc/User_Credentials_H.htm)*
page.

Refer to [Establish a Connection to a Target
System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
for more information.

**NOTE:** If a user adds a request based on this template and does not
select a connection ID, the default connection assigned to the Integrate
Template is used for the request.

User Credentials

Click to open the <span style="font-style: italic;">[User
Credentials](../../../Platform/Common/Page_Desc/User_Credentials_H.htm)</span>
page to add Login credentials for the current user to track that user’s
updates posted to the target system related to requests based on this
template.

Credentials Detected

If enabled, the user name and password have been detected based on the
user credentials setting.

If disabled, the credentials have not been detected and must be added
for the request to post successfully.

Setup

Connection

Displays target ERP system used to record the template. If importing a
template from Integrate, set the Type to match the posting type of the
template. A Connection must be selected when creating a custom template
(i.e., when the Type is set to Custom Setup); however, it does not apply
to the template and is ignored.

Roles

Click to open the*[Template (Role)](Template_Role_H.htm)* page to add,
edit and delete roles assigned to the template.

**NOTE:** The count on this icon indicates the number of roles assigned
to the template. Global roles with the Auto Copy option set on the
*[Roles](Roles_H.htm)* page are automatically added to a template when
it is created. Refer to [Add a Global
Role](../Config/Add_a_Global_Role.htm) for more information.

Org Units

Click to open the *[Template (Org Units)](Template_Org_Units_H.htm)*
page to add, edit and delete Org Units assigned to the template. Org
units are optional for templates.

**NOTE:** The count on this icon indicates the number of Org Units
assigned to the template. Refer to [Add Org Units to a
Template](../Use_Cases/Set_up_Org_Units.htm#Add_Org_Units_to_a_Template)
for more information.

Users

Click to open the *[Template (Users)](Template_Users_H.htm)* page to
add, edit or delete users who have been granted access to the template.
The user who created the template is automatically assigned to the
template and to all the roles.

**NOTE:** The count on this icon indicates the number of users granted
access to the template. The user who created the template is
automatically assigned to the template and to all the template’s roles.

Actions

Record

Click to launch the local target ERP system environment where script
recording for the template occurs. The Record icon is only available if
creating a GUI Script or a BDC Script template. When the Record icon is
clicked, if an Integrate Template ID is set, dspCompose™ overrides the
Template ID with the recording. Because this Integrate template may also
be used in Integrate, take special care when re-recording (and thus
modifying) a template that has been imported from Integrate.

**NOTE:** This option does not display if the template is active.

Generate

Click to generate the template when a template recording is complete.
dspCompose™ imports the recording for the template into Integrate for
posting and creates all the necessary data entry pages in dspCompose™. A
template cannot be activated until it is generated. The Record icon is
only available if creating a GUI Script or a BDC Script template.

**NOTE:** This option does not display if the template is active.

Generate Custom

Click to generate the custom template. This icon only displays if
creating a custom template (as in, when the Type is set to Custom
Setup).

## <span id="Configuration_Tab"></span>Configuration tab

Field

Description

Template Settings

Template Team

Displays name of team to which the template is assigned.

Post Message Tables

Click to open the *[Template (Post Message
Tables)](Template_Post_Message_Tables.htm)*page to add, edit and delete
tables that store posting feedback.

Retention Params

Click to open the *[Template (Request
Retention)](Template_Request_Retention.htm)* page to edit how long a
request with a specific status is retained before it is archived.

Objects

Click to open the *[Template (Objects)](Template_Objects.htm)* page to
add, edit and delete tables, stored procedures and views that are
automatically created in the cMass\_Data database when a template is
generated.

Events

Click to open the *[Template (Events)](Template_Events.htm)* page to
configure events that trigger rules to run for the template.

External Request Creation

External Request Scenarios

Click to open the [*Template (External Request
Scenario)*](Template_External_Request_Scenario.htm) page to add, edit
and delete external request scenarios, including external request
scenarios that create Excel-initiated requests.

**NOTE:** The number on the icon represents the number of external
request scenarios that exist for the template.

Posting

Messages To Return

This field is not used.

Integrate Template ID

Displays name of Integrate template used as the dspCompose™ template
recording.

Integrate Process ID

Displays the ID for the process generated by Integrate and used to post
request data to the target ERP system. Click the link to view the
Process in Integrate.

Script ID

Displays name of GUI or BDC script (as in, recording) used in the
template.

 

## <span id="Advanced_Tab"></span>Advanced tab

<div class="use">

Use this tab to:

  - [Regenerate Data
    Objects](../Use_Cases/Data_Objects.htm#Regenerate_Data_Objects)
  - [Set Force Reject
    Severity](../Use_Cases/Set_Force_Reject_Severity.htm)
  - [Set Org Unit Assignment Security for a
    Request](../Use_Cases/Request_Org_Unit_Assignments.htm#Set_Org_Unit_Assignment_Security_for_a_Request)
  - [Create a Custom
    Template](../Use_Cases/Create_a_Custom_Template_dspCompose.htm)

</div>

Field

Description

Validation

Enable List Box Validation

If enabled, dspCompose™ validates the values entered on the data entry
pages of the request that have a list or a combo box. When the user
clicks the Validate button on the *[Request
(Roles)](Request_Roles_H.htm)*page, dspCompose™ ensures that the values
that have been entered or selected on the data entry pages are contained
in the list boxes assigned to the data entry pages. Records that fail
this validation fail with a severity of Error. The default for this
setting is set on the*[Parameters](Parameters.htm)*page.

Enable Required Validation

If enabled, dspCompose™ validates that all required fields of data type
nvarchar on data entry pages of the request contain values. Records with
blank required fields fail with a severity of Error. dspCompose™ runs
the validation when the user clicks the Validate button on the *[Request
(Roles)](Request_Roles_H.htm)* page. The default for this setting is set
on the *[Parameters](Parameters.htm)* page.

**NOTE:** Validations are not run on required fields with data types
other than nvarchar.

Enable Check Box Validation

If enabled, dspCompose™ validates that the values selected on data entry
pages of the request for a check box are the values in the table
corresponding to the proper check box format set on the column property.
Records that fail this validation fail with a severity of Error.
dspCompose™ runs the validation when the user clicks the Validate button
on the *[Request (Roles)](Request_Roles_H.htm)* page. The default for
this setting is set on the *[Parameters](Parameters.htm)* page.

Force Reject Severity

If enabled, dspCompose™ rejects data entry records that fail a
validation whose severity meets or exceeds the Force Reject Severity.
These records cannot be approved by the Review role and are
automatically rejected and sent back to the Data role for correction.
 If no Force Reject Severity is set, all data entry records can be
rejected or approved by Review role users. The default for this setting
is set on the *[Parameters](Parameters.htm)* page.

Org Unit Security Level

Displays value that represents actions that may be performed on Org Unit
Values when a request is created. Values are:

  - **OrgUnit Values Available For Assignment –** All of the individual
    Org Unit values possible for the request are available for
    assignment to the request, but no assignments are assigned by
    default.
  - **User Assignments, Defaulted Change Allowed –** All of the
    individual Org Unit assignments available to the user creating the
    request are assigned to the request by default, but may be
    unassigned.
  - **User Assignments Defaulted, No Change Allowed –** All of the
    individual Org Unit assignments available to the user are assigned
    to the request and cannot be unassigned. If this option is selected,
    the Select All, Unselect All, and Reset Defaults button do not
    display on the *[Request (Org Unit
    Assignments)](Request_Org_Unit_Assignments.htm)* page.

The default value is configured on the
*[Parameters](Parameters.htm)*page.

Only Show Org Unit Values Assigned to Requester

If enabled, Org Unit values presented at the request level are based on
the requester’s Org Unit assignments. If disabled, Org Unit values
presented at the request level are based on all users’ Org Unit
assignments from users assigned to the template.

Archive Settings

Template Archive Web App ID

Displays data source that contains the Template Archive Page ID.

Template Archive Page ID

Displays page ID automatically set for a template when the template is
processed and when roles are configured. If non-custom review roles are
used, the Template Archive Page ID is set to the system-generated page.

Custom Archive Tables

Click to open the*[Template (Archive
Settings)](Template_Archive_Settings.htm)*page to add, edit and delete
custom archive tables. When a request is archived, the data is selected
out of the active table(s) and written to the archive table(s). Data is
only inserted into the custom archive tables; deletes and updates are
not performed.

Maintenance

Regenerate Data Objects

Click to update all system-generated objects based on changes made to
the data entry page for the template.

**NOTE:** This icon is only available while in Developer Mode.

**NOTE:** This icon does not display for custom templates (i.e., when
the Type is set to Custom Setup).

Reset

Reset Status

Click to reset the status to Procedure Completed. This icon is only
active while in Developer Mode.

Developer

Developer Mode

If enabled, a user can make changes to an active template with active
requests. If disabled, no changes can be made to an active template with
active requests.

Delete All Requests

Click to delete all requests that currently use this template so that
the template can be deleted. In order to delete a template, all requests
for the template must first be deleted.
