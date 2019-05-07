+++
title = 'Request Post Workflow Notification'
solution = 'Master Data Management'
+++

# Request Post Workflow Notification

<div class="use">

Use this page to Configure Users who Receive Workflow Notifications for
Successful or Failed Postings at the Request Role Level.

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspConduct \>
    </span>**Requests** in the *Navigation* pane.
2.  Click the **Roles** icon for a request.
3.  Click <span style="font-weight: bold;">Vertical View</span> for the
    Post role.
4.  Click the **Request Post Workflow Notification** button.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>USER ID</p></td>
<td><p>Displays the ID of the user who receives notifications when a posting succeeds or fails.</p>
<p><strong>NOTE:</strong> This user can be registered in the platform or can be an external user.</p></td>
</tr>
<tr class="odd">
<td><p>USER NAME</p></td>
<td><p>Displays the user name associated with the user ID in the platform, or the user name entered on for the external user.</p></td>
</tr>
<tr class="even">
<td><p>EMAIL ADDRESS</p></td>
<td><p>Displays the email address associated with the user ID in the platform, or the email address entered for the external user.</p></td>
</tr>
<tr class="odd">
<td><p>LANGUAGE ID</p></td>
<td><p>Displays the language used in the workflow message.</p>
<p><strong>NOTE:</strong> Workflow messages must have been added for that language to the <a href="Category_Workflow_Language_Message_H.htm">Category Workflow Language Message</a> page for the Posted and Posted with Errors event. If they are not added, the notifications are not sent. Refer to <a href="../Config/Create_Language-specific_Workflow_Messages_for_a_Category.htm">Create Language-specific Workflow Messages</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>SEND POST SUCCESS</p></td>
<td><p>If enabled, the user receives notifications when the posting status is Success.</p></td>
</tr>
<tr class="odd">
<td><p>SEND POST FAIL</p></td>
<td><p>If enabled, the user receives notifications when the posting status is Failure.</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If enabled, the user receives notifications.</p>
<p>The check box is enabled by default.</p>
<p><strong>NOTE:</strong> If a user is added at the scenario role level, this check box must be disabled for that user on this page if the user must not receive these types of notifications.</p></td>
</tr>
</tbody>
</table>
