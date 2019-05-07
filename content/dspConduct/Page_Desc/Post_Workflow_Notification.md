+++
title = 'Post Workflow Notification'
solution = 'Master Data Management'
+++

# Post Workflow Notification

<div class="use">

Use this page to [Configure Users who Receive Workflow Notifications for
Successful or Failed Postings at the Scenario Role
Level.](../Config/Send_Workflow_Notifications_when_a_Post_Fails_or_Succeeds.htm#Configure_Users_who_Receive_Workflow_Notifications_at_the_Scenario_Role_Level)

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspConduct \>
    </span>**Design** in the *Navigation* pane.
2.  Click the **Scenarios** icon for a category.
3.  Click the **Roles** icon for a scenario.
4.  Click **Vertical View** for the Post role.
5.  Click the **Post Workflow Notification** icon.

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
<td><p>NAME</p></td>
<td><p>Displays the user name associated with the user ID in the platform, or the user name entered on for the external user.</p></td>
</tr>
<tr class="even">
<td><p>E MAIL ADDRESS</p></td>
<td><p>Displays the email address where notifications are sent for the user ID in the platform, or the email address entered for the external user.</p></td>
</tr>
<tr class="odd">
<td><p>LANGUAGE ID</p></td>
<td><p>Displays the language used in the workflow message.</p>
<p><strong>NOTE:</strong> Workflow messages must have been added for that language to the <a href="Category_Workflow_Language_Message_H.htm">Category Workflow Language Message</a> page for the Posted and Posted with Errors event. If they are not added, the notifications are not sent. Refer to <a href="../Config/Create_Language-specific_Workflow_Messages_for_a_Category.htm">Create Language-specific Workflow Messages</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>SEND POST SUCCESS</p></td>
<td><p>If enabled, the user receives notifications when the posting status is Success.</p>
<p><strong>NOTE:</strong> This setting can be enabled or disabled for individual users at the request role level.</p></td>
</tr>
<tr class="odd">
<td><p>SEND POST FAIL</p></td>
<td><p>If enabled, the user receives notifications when the posting status is Failed.</p>
<p><strong>NOTE:</strong> This setting can be enabled or disabled for individual users at the request role level.</p></td>
</tr>
</tbody>
</table>
