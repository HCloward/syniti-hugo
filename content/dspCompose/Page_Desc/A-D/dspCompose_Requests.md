+++
title = 'dspCompose Requests H'
solution = 'Data Quality'
+++

# dspCompose Requests H

[dspCompose Requests V](dspCompose_Requests.htm#dspCompose__Requests_V)

<div class="use">

[View Your Active Requests
Details.](../Use_Cases/View_Your_Active_Requests_Details.htm)

</div>

To access this page, click the black dspCompose Requests tab in the
Quick
Panel.

|               |                                                                                                                                                                                                                                                                                                                          |
| ------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field         | Description                                                                                                                                                                                                                                                                                                              |
| Requests      | Click to open the <span style="font-style: italic;">[Request](Request_H.htm)</span> page to view additional request details and access functionality related to org units and external role contacts for all requests.<span> </span>                                                                                     |
| REQUEST ID    | Displays unique number that identifies the request.                                                                                                                                                                                                                                                                      |
| STATUS        | Displays icon that represents the <span id="dspCompose Request Status" class="popUpLink">\>request status</span> of an active request.                                                                                                                                                                                   |
| Roles         | Click to open the <span style="font-style: italic;">[Request (Roles)](Request_Roles_H.htm)</span> page, where request data is entered, reviewed and posted. If a request uses both external contacts and Org Units, the Roles icon is not active until both the External Contacts and the Org Units have been confirmed. |
| Request Data  | Click to view all data entered for the request regardless of the posting status.                                                                                                                                                                                                                                         |
| DESCRIPTION   | Displays brief description of the request.                                                                                                                                                                                                                                                                               |
| TEMPLATE NAME | Displays template name used for the request. Click the link to open the <span style="font-style: italic;">[Templates](Templates_H.htm)</span> page to access the template on which the request is based.                                                                                                                 |

## <span id="dspCompose__Requests_V"></span>dspCompose Requests V

[dspCompose Requests H](#)

Field

Description

Requests

Click to open the
<span style="font-style: italic;">[Request](Request_H.htm)</span> page
to view additional request details and access functionality related to
org units and external role contacts for all requests.<span> </span>

Request Properties

Description

Displays brief description of the request.

Template Name

Displays template name used for the request. Click the link to open the
[Templates](Templates_H.htm)  page to access the template on which the
request is based.

Connection
ID

<span style="font-size: 11.0pt;line-height: 107%;font-family: Arial, sans-serif;">Displays
the target ERP system connection that is used to post the data during
the posting role. dspCompose™ can post to multiple target ERP system
instances. The connections are set up in Common.</span>

Refer to [Establish a Connection to a Target
System](../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm)
for more information.

Org Units

Click to open the *[Request (Org Unit
Assignments)](Request_Org_Unit_Assignments.htm)* page to view a list of
org unit values used in the request. Depending on how org units are
configured for the template (using the Org Unit Security Level set on
the Advanced tab of the *[Templates](Templates_H.htm)* page’s
<span style="font-size: 11.0pt;line-height: 107%;font-family: Arial, sans-serif;font-style: italic;">Vertical</span>
View), users may be able to assign and unassign org units from the
request.

This icon is not active:

  - If org units are not set up for the template used by the request, or
  - After org units are confirmed for the request (i.e., after a user
    clicks the Confirm Org Units icon).

Org Units Assigned

Click to open the *[Request (Org Units
Assigned)](Request_Org_Units_Assigned.htm)* page to view the org units
assigned to the request. This icon is active once Org Units Assigned are
set up for the assigned template.  

Request Status

Displays the current
<span id="dspCompose Request Status" class="popUpLink">status</span> of
the request<span>. </span>

Posted On

Displays the date the request was posted. If the field is blank, the
request has not yet been posted.

Posted
By

<span style="font-size: 11.0pt;line-height: 107%;font-family: Arial, sans-serif;">Displays
the user ID of the user who posted the request.</span>

Process Request

Request Data

Click to view all data entered for the request regardless of the posting
status. Verify target data imported and the fields mapped correctly.

External Role Contacts

Click to open the [Request (External Role
Contacts)](Request_External_Role_Contacts.htm) page to configure the
name, email address and language for external contacts who are assigned
to an External Data role within the request. This icon is only available
if the template upon which the request is based has an External Data
role.

The icon displays the number of external role contacts that have a valid
email address. Records that contain only a Role ID are not included in
the count.

Roles

Click to open the *[Request (Roles)](Request_Roles_H.htm)* page, where
request data is entered, reviewed and posted. If a request uses both
external contacts and org units, the Roles icon is not active and the
request cannot be processed until both the external contacts and the org
units have been confirmed.

Data Archive

Archive Page ID

Click to view an audit trail/log of what occurs when the post process is
run for a request, i.e., a posting summary for the request.

Rejection Archive

Click to view an archive of all rejected roles, including the reason for
rejection and the user who rejected the role. This icon is active if any
request records have been rejected by the Review role.
