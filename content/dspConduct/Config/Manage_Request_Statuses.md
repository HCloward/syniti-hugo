+++
title = 'Manage Request Statuses Overview'
solution = 'Master Data Management'
+++

# Manage Request Statuses Overview

The <span style="font-style: italic;">[Request
Status](../Page_Desc/Request_Status.htm)</span> page lists the default
statuses installed with dspConduct™. Default status cannot be edited or
deleted.

Default statuses have settings configured for archiving a request,
editing a request, and allowing role access to the request.

If the ARCHIVABLE check box on the
<span style="font-style: italic;">Request Status</span> page is enabled
for a status, a request in the status can be archived. By default, a
request is archived if it remains in the same status for 30 days. If the
ARCHIVABLE check box is disabled, a request in this status is not
archived, even after the default setting of 30 days has passed.

<span style="font-weight: bold;">NOTE</span>: This setting can be
updated at the category level. Refer to [Set the Days Active for a
Request Status](Set_the_Days_Active_for_a_Request_Status.htm) for more
information.

<span style="font-weight: bold;">NOTE</span>: Setting the request status
to Cancelled, Deleted or Duplicate Request must be controlled on the
Content WebApp's Request page. dspConduct™ does not set these statuses.

If the EDITABLE check box on the
<span style="font-style: italic;">Request Status</span> page is enabled
for a request status, a Role Processor with access to the request can
edit the request based on the role’s type when the request is in that
status. If the EDITABLE check box is disabled, a request in this status
is read only. No actions can be performed on the request until it moves
to a request status with the EDITABLE check box enabled.

If the ROLE ACCESS check box on the
<span style="font-style: italic;">Request Status</span> page is enabled
for a status, a request in the status can be processed by a role. The
Finish and Validate buttons are active when the request is being
processed by the Application role. The Reset, Validate, and Reviewer
Workbench buttons are active when the request is being processed by the
Review role. The Finish button is active for the Post role. If ROLE
ACCESS is disabled, these buttons are disabled and a role cannot process
the request until it moves to a status where the ROLE ACCESS check box
is enabled.

<table>
<tbody>
<tr class="odd">
<td><p>Status</p></td>
<td><p>Description</p></td>
<td><p>Editable</p></td>
<td><p>Archivable</p></td>
<td><p>Role Access</p></td>
</tr>
<tr class="even">
<td><p>Draft</p></td>
<td><p><span style="font-size: 11.0pt;line-height: 107%;font-family: Arial, sans-serif;">The request has been created in the Content WebApp but has not been submitted.</span></p></td>
<td><p>Yes</p></td>
<td><p>No</p></td>
<td><p>No</p></td>
</tr>
<tr class="odd">
<td><p>Cancelled</p></td>
<td><p>The request will not be posted because it has been marked for cancellation.</p></td>
<td><p>Yes</p></td>
<td><p>Yes</p></td>
<td><p>Yes</p></td>
</tr>
<tr class="even">
<td><p>Deleted</p></td>
<td><p>The request will never be posted because it has been marked for deletion.</p></td>
<td><p>No</p></td>
<td><p>Yes</p></td>
<td><p>No</p></td>
</tr>
<tr class="odd">
<td><p>Duplicate Request</p></td>
<td><p>The request is a duplicate of another request already in the system.</p></td>
<td><p>No</p></td>
<td><p>Yes</p></td>
<td><p>No</p></td>
</tr>
<tr class="even">
<td><p>Scheduled</p></td>
<td><p>The request is scheduled to be posted at the date and time set on the <span style="font-style: italic;"><a href="../Page_Desc/Request_Group_Post.htm">Request Group Post</a></span> page.</p></td>
<td><p>No</p></td>
<td><p>No</p></td>
<td><p>Yes</p></td>
</tr>
<tr class="odd">
<td><p>Posted</p></td>
<td><p>The Request has been posted. All Integrate processes have completed posting, but the Post role has not been finished.</p></td>
<td><p>Yes</p></td>
<td><p>No</p></td>
<td><p>Yes</p></td>
</tr>
<tr class="even">
<td><p>Posted with Errors</p></td>
<td><p>At least one posting process has failed. All Integrate processes have completed posting, but the Post role has not been finished.</p></td>
<td><p>Yes</p></td>
<td><p>No</p></td>
<td><p>Yes</p></td>
</tr>
<tr class="odd">
<td><p>Posting Started</p></td>
<td><p>A user clicked the Group Post or Post icons on the <span style="font-style: italic;"><a href="../Page_Desc/Request_Group_Post.htm">Request Group Post</a></span> or <a href="../Page_Desc/Request_Post_Process.htm">Request Post Process</a> page but the posting processes have not completed yet. .</p></td>
<td><p>No</p></td>
<td><p>No</p></td>
<td><p>No</p></td>
</tr>
<tr class="even">
<td><p>Request in process</p></td>
<td><p>This request is in process and has not been fully posted.</p></td>
<td><p>Yes</p></td>
<td><p>No</p></td>
<td><p>Yes</p></td>
</tr>
<tr class="odd">
<td><p>Finish Processing</p></td>
<td><p>This request has been posted and is awaiting finished data download.</p></td>
<td><p>No</p></td>
<td><p>No</p></td>
<td><p>No</p></td>
</tr>
<tr class="even">
<td><p>Finish Failed</p></td>
<td><p>This request has been posted but the downloading of finished data failed.</p></td>
<td><p>Yes</p></td>
<td><p>Yes</p>
<p> </p></td>
<td><p>Yes</p>
<p> </p></td>
</tr>
<tr class="odd">
<td><p>Finished</p></td>
<td><p>This request has been posted and the finished data has been downloaded.</p></td>
<td><p>No</p></td>
<td><p>Yes</p></td>
<td><p>No</p></td>
</tr>
</tbody>
</table>

A user can add a custom status, and set the archive, edit, and role
access settings for that status.

To work with request statuses:

  - [Add a Custom Request
    Status](../Use_Cases/Add_a_Custom_Request_Status.htm)
  - [Set the Days Active for a Request
    Status](Set_the_Days_Active_for_a_Request_Status.htm)
