+++
title = 'Request H'
solution = 'Data Quality'
+++

# Request H

[Requests V](#Request_V_All_Tabs)

<span style="font-weight: bold;">NOTE:</span> This page also displays
when the user clicks Rejection Archive on the
<span style="font-style: italic;">Request</span> page's
<span style="font-style: italic;">Vertical</span> View. View the [field
descriptions for the
page](#Request__Accessed_via_the_Rejection_Archive_icon_) when it is
accessed in this manner.

<div class="use">

Use this page to:

  - [Create Requests](../Use_Cases/Create_Requests.htm)
  - [Validate a Role](../Use_Cases/Validate_a_Role.htm)
  - [Reset a Role](../Use_Cases/Reset_a_Role.htm)
  - [Reject a Role](../Use_Cases/Review_Request_Data.htm#Reject_a_Role)
  - [Post Request Data to a Target ERP
    System](../Use_Cases/Post_Request_Data_to_a_Target_ERP_System.htm)

</div>

To access this page, select **dspCompose \> Requests** in the
*Navigation* pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Confirm External Contacts</p></td>
<td><p>Click to confirm external contacts assigned to the request. Once External Contacts and Org Units (if applicable) are confirmed, the request becomes active.</p>
<p>dspCompose™sends an email with an Excel spreadsheet attached that contains request data to users configured as external contacts for the External Data role. This user updates the spreadsheet and attaches it to an email and sends it back to dspCompose™.</p>
<p>The icon is active if the request uses a template with an External Data role and if at least one external contact is configured with a valid email address for the request.</p>
<p>If the request has both external contacts and Org Units assigned, Org Units must be confirmed before external contacts.</p></td>
</tr>
<tr class="odd">
<td><p>Confirm Org Units</p></td>
<td><p>Click to confirm the Org Units assigned to the request. dspCompose™ removes Org Unit values from a request that do not have the ASSIGNED check box enabled on the <em>Request (Org Unit Assignments)</em> page. Once confirmed, these values cannot be changed. Once Org Units and External Contacts (if applicable) are confirmed, the request becomes active.</p>
<p>The icon is active if the request uses a template where Org Units are configured.</p>
<p>If the request has both external contacts and Org Units assigned, Org Units must be confirmed before external contacts.</p></td>
</tr>
<tr class="even">
<td><p>REQUEST ID</p></td>
<td><p>Displays unique number that identifies the request.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays brief description of the request.</p></td>
</tr>
<tr class="even">
<td><p>TEMPLATE</p></td>
<td><p>Displays template name used for the request. Click link to open the<span style="font-family: Arial, sans-serif;font-style: italic;">Templates</span>page to access the template on which the request is based.</p></td>
</tr>
<tr class="odd">
<td><p>Status</p></td>
<td><p>Displays icon that represents the<span id="dspCompose Request Status" class="popUpLink"> request status</span> of an active request.</p></td>
</tr>
<tr class="even">
<td><p>Roles</p></td>
<td><p>Click to open the <em><a href="Request_Roles_H.htm">Request (Roles)</a></em> page, where request data is entered, reviewed and posted. If a request uses both external contacts and Org Units, the Roles icon will not be active until both the External Contacts and the Org Units have been confirmed.</p></td>
</tr>
<tr class="odd">
<td><p>Org Units</p></td>
<td><p>Click to open the <a href="Request_Org_Unit_Assignments.htm">Request (Org Unit Assignments)</a> page to view a list of Org Units values used in the request. Depending on how Org Units are configured for the template (using the Org Unit Security Level set on the Advanced tab of the<em><a href="Templates_H.htm">Templates</a></em> page’s <em>Vertical</em> View), users may be able to assign and unassign Org Units from the request. The icon is not active if Org Units are not set up for the template used by the request. Once Org Units are confirmed for the request (i.e., Confirm Org Units button is clicked), the Org Units icon is no longer available.</p></td>
</tr>
<tr class="even">
<td><p>Org Units Assigned</p></td>
<td><p>Click to open the <em><a href="Request_Org_Units_Assigned.htm">Request (Org Units Assigned)</a></em> page to view the Org Units assigned to the request This icon is active once Org Units Assigned are set up for the assigned template.</p></td>
</tr>
<tr class="odd">
<td><p>External Role Contacts</p></td>
<td><p>Click to open the <em><a href="Request_External_Role_Contacts.htm">Request (External Role Contacts)</a></em> to configure the name, email address and language for external contacts who are assigned to an External Data role within the request. This icon is only available if the template upon which the request is based has an External Data role.</p>
<p>The icon displays the number of external role contacts that have a valid email address. Records that contain only a Role ID are not included in the count.</p></td>
</tr>
<tr class="even">
<td><p>Request Data</p></td>
<td><p>Click to view all data entered for the request regardless of the posting status. Verify target data imported and the fields mapped correctly.</p></td>
</tr>
</tbody>
</table>

## <span id="Request_V_All_Tabs"></span>Request V All Tabs

[Requests H](Request_H.htm)

This page contains the following tabs:

  - [General tab](#General_Tab1)
  - [Change Status tab](#Change_Status_Tab)

## <span id="General_Tab1"></span>General tab

<div class="use">

Use this tab to [Create Requests](../Use_Cases/Create_Requests.htm).

</div>

Field

Description

Confirm External Contacts

Click to confirm external contacts assigned to the request. Once
External Contacts and Org Units (if applicable) are confirmed, the
request becomes active.

dspCompose™ sends an email with an Excel spreadsheet attached that
contains request data to users configured as external contacts for the
External Data role. This user updates the spreadsheet and attaches it to
an email and sends it back to dspCompose™.

The icon is active if the request uses a template with an External Data
role and if at least one external contact is configured with a valid
email address for the request.

If the request has both external contacts and Org Units assigned, Org
Units must be confirmed before external contacts.

Confirm Org Units

Click to confirm the Org Units assigned to the request. dspCompose™
removes Org Unit values from a request that do not have the ASSIGNED
check box enabled on the *Request (Org Unit Assignments)* page. Once
confirmed, these values cannot be changed. Once Org Units and External
Contacts (if applicable) are confirmed, the request becomes active.

The icon is active if the request uses a template where Org Units are
configured.

If the request has both external contacts and Org Units assigned, Org
Units must be confirmed before external contacts.

Request Properties

Description

Displays brief description of the request.

Template

Displays template name used for the request.

Connections

Click to open the *[Request Connections](Request_Connections.htm)* page
to set the target ERP system connection(s) that are used to post the
data during the posting role. dspCompose™ can post to multiple target
ERP system instances.

Refer to [Establish a Connection to a Target
System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
for more information.

**NOTE:** If a user adds a request based on this template and does not
select a connection ID, the default connection assigned to the Integrate
Template is used for the request.

Org Units

Click to open the [*Request (Org Unit
Assignments)*](Request_Org_Unit_Assignments.htm) page to view a list of
Org Units values used in the request. Depending on how Org Units are
configured for the template (using the Org Unit Security Level set on
the Advanced tab of the *[Templates](Templates_H.htm)* page’s *Vertical*
View), users may be able to assign and unassign Org Units from the
request. The icon is not active if Org Units are not set up for the
template used by the request. Once Org Units are confirmed for the
request (i.e., Confirm Org Units button is clicked), the Org Units icon
is no longer available.

Org Units Assigned

Click to open the [*Request (Org Units
Assigned)*](Request_Org_Units_Assigned.htm) page to view the Org Units
assigned to the request. This icon is active once Org Units Assigned are
set up for the assigned template.  

Request Status

Displays the current status of the request, as indicated by the Status
icon on the Horizontal View. Values are: Cancelled, Deleted, Finished,
Posted, Posted With Errors, Posting, Posting Scheduled and Request In
Process.

Posted On

Displays the date the request was posted.

Posted By

Displays the user ID of the user assigned to the Post role who clicked
the Finish button on the <span style="font-style: italic;">[Request
(Post)](Request_Post.htm)</span> page.

Created From Rejected Request ID

Displays name of original request if only part of the original request
data was approved and posted to the target ERP system and the current
request was created with the rejected data. This field is only available
if part of the original request data was approved.

Process Request

Request Data

Click to view all data entered for the request regardless of the posting
status. Verify target data imported and the fields mapped correctly.

External Role Contacts

Click to open the *[Request (External Role
Contacts)](Request_External_Role_Contacts.htm)* to configure the name,
email address and language for external contacts who are assigned to an
External Data role within the request. This icon is only available if
the template upon which the request is based has an External Data role.

The icon displays the number of external role contacts that have a valid
email address. Records that contain only a Role ID are not included in
the count.

Roles

Click to open the *[Request (Roles)](Request_Roles_H.htm)* page, where
request data is entered, reviewed and posted. If a request uses both
external contacts and Org Units, the Roles icon will not be active and
the request cannot be processed  until both the External Contacts and
the Org Units have been confirmed.

Data Archive

Archive Page ID

Click to view an audit trail/log of what occurs when the post process is
run for a request, as in, a posting summary for the request.

Rejection Archive

Click to view an archive of all rejected roles, including the reason for
rejection and the user who rejected the role. This icon is only
activated if any request records have been rejected by the Review role.

Finish Download

Finish Download Status

Click to open the *[Request Role Finish
Monitor](Request_Role_Finish_Monitor.htm)* page, which displays every
action that takes place during the Post role’s Final Finish download of
data from a source to a target. This icon is only enabled once the
Finish button for the Post role has been clicked.

## <span id="Change_Status_Tab"></span>Change Status tab

<div class="use">

Use this page to [Change Request
Status](../Use_Cases/Change_Request_Status.htm).

</div>

Field

Description

Change Request Status

Cancel Request

Click to cancel the request. Cancelled requests are archived using the
retention interval set on the template used by the request.

Delete Request

Click to delete the request, i.e., set the request status
as<span style="font-family: Arial, sans-serif;font-style: italic;">Deleted</span>.
A service page runs once daily to delete requests with a status of
Deleted.

Reset

Reset Request

Click to reset the request, which overrides the current state of the
request and resets it for processing. This should only be used if an
error occurred during processing which left the request in an unusable
state.

### <span id="Request__Accessed_via_the_Rejection_Archive_icon_"></span>Request (Accessed via the Rejection Archive icon)

<div class="use">

Use this page to view rejection history for a request when [rejecting a
role.](../Use_Cases/Review_Request_Data.htm#Reject_a_Role)

</div>

|                  |                                                                                                                                              |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| Field            | Description                                                                                                                                  |
| ROLE ID          | Displays the role ID of the user who rejected the request.                                                                                   |
| REJECTED BY      | Displays the user ID of the user who rejected the request.                                                                                   |
| REJECTED ON      | Displays the date the request was rejected.                                                                                                  |
| REJECTION REASON | Displays the reason entered by the user for rejecting the request on the <span style="font-style: italic;">[Reject](Reject.htm)</span> page. |
