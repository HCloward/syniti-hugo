+++
title = 'Set Up Workflow Messages'
solution = 'Data Quality'
+++

# Set Up Workflow Messages

Requests are workflow-enabled, meaning that each user assigned to a role
in a request can receive a notification when the role has work assigned.
A workflow is a notification method called during an event, in this
case, when a role is finished.

When one stage of work has been completed for a request, dspCompose™
sends an email and displays a notification pop-up to that user from
within dspCompose™ notifying all members of the next dependent role or
roles they have tasks to complete. The email contains a link to trigger
specific events and to launch the relevant page in dspCompose™.

Workflow messages can be configured. Refer to [Configure Workflow
Messages](Configure_Workflow_Messages) for more information.

<span style="font-weight: bold;">NOTE:</span> Workflow messages can be
configured for the languages that display in the LANGUAGE ID column.
These languages are defined as active in the platform.

dspCompose™ can be configured to use the recipient’s user name or email
address in the workflows.

To view the list of delivered workflow messages:

1.  Select <span class="Body">**Configuration \> Workflow
    Message**</span> on the *Navigation* pane.
2.  Click <span class="Body">**Messages**</span> for a language.

**NOTE**: The **EVENT** column lists the event that triggers the message
to be sent.

For example, when a user finishes a role by clicking **Finish** on the
*Request (Roles)* page, the Finish event is triggered, and an email
notification and a pop-up notification from within dspCompose™ are sent
to the next person(s) responsible for subsequent role(s). The email and
notification contain the workflow message associated with the Finish
event.

Workflow messages must be enabled for a user.

To enable workflow messages:

1.  Select **Configuration \> Users** on the *Navigation* pane.
2.  Click the **SEND WORKFLOW** check box to enable workflow messaging
    for a user.

To set workflow message to use the recipient’s email or user name:

1.  Select **Configuration \> Parameters** on the *Navigation* pane.
2.  Click the **Use UserID in Workflow** check box to enable it or
    disable it.

**NOTE**: If the Use UserID in Workflow check box is enabled,
dspCompose™ uses the recipient’s user name when sending workflow
emails, making the workflow semi-anonymous. If disabled, dspCompose™
uses the recipient’s email address.

The following tables lists the type of workflow messages and the role(s)
that receives them.

<table>
<tbody>
<tr class="odd">
<td><p>Event</p></td>
<td><p>Role that Receives Workflow</p></td>
</tr>
<tr class="even">
<td><p>All records in a request are rejected.</p></td>
<td><p>Initial Data role</p></td>
</tr>
<tr class="odd">
<td><p>Request is canceled.</p></td>
<td><p>Initial Data role</p></td>
</tr>
<tr class="even">
<td><p>Request is deleted.</p></td>
<td><p>Initial Data role</p></td>
</tr>
<tr class="odd">
<td><p>Initial Role<span> </span> is ready to be processed in an External Request Scenario that does not contain an External Data role</p></td>
<td><p>Initial Data role</p></td>
</tr>
<tr class="even">
<td><p>New request is created automatically from rejected records from a partial approval.</p></td>
<td><p>Initial Data role</p></td>
</tr>
<tr class="odd">
<td><p>Role is reset.</p></td>
<td><p>Any Data role that worked on the request</p></td>
</tr>
<tr class="even">
<td><p>Role is finished.</p></td>
<td><p>Next role to be processed in the workflow</p></td>
</tr>
<tr class="odd">
<td><p>Role validated.</p></td>
<td><p>Any Data role that worked on the request.</p>
<p>If a validation threshold is set and the number of validation failures exceeds the validation threshold, the validation threshold contact also receives a workflow message.</p></td>
</tr>
<tr class="even">
<td><p>External request scenario with External Data role is ready to be processed</p></td>
<td><p>External Data role</p></td>
</tr>
<tr class="odd">
<td><p>External Role data entry fails validation.</p></td>
<td><p>External Data role</p></td>
</tr>
<tr class="even">
<td><p>Role is made active and ready to be processed</p></td>
<td><p>Next role in the workflow.</p></td>
</tr>
</tbody>
</table>
