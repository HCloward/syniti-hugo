+++
title = 'Category Workflow Language Message H'
solution = 'Data Quality'
+++

# Category Workflow Language Message H

[Category Workflow Language Message
V](#Category_Workflow_Language_Message_V)

<div class="use">

Use this page to [Edit Category Language-specific
Messages](../Config/Edit_Category_Language_specific_Messages.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspConduct \>
    </span>**Design**<span>in</span> the *Navigation* pane.
2.  Click **Vertical View** for a category.
3.  Click the **Workflow Messages** icon.
4.  Click the <span style="font-weight: bold;">Messages</span> icon for
    a language.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Enable</p></td>
<td><p>Click to enable the selected message(s) in the category.</p></td>
</tr>
<tr class="odd">
<td><p>Disable</p></td>
<td><p>Click to disable the selected message(s) in the category. This message(s) is not sent to users in the category.</p></td>
</tr>
<tr class="even">
<td><p>EVENT</p></td>
<td><p>Displays the event that triggers the workflow email to be sent.</p>
<p><strong>NOTE:</strong> The name must be unique to the category. The Event name cannot be updated for default events.</p></td>
</tr>
<tr class="odd">
<td><p>SUBJECT</p></td>
<td><p>Displays the subject line of workflow email. A value preceded and followed by # is a dynamic substitution value for replacement at run time.</p></td>
</tr>
<tr class="even">
<td><p>MESSAGE</p></td>
<td><p>Displays the body text within the workflow email. A value preceded and followed by # is a dynamic substitution value for replacement at run time.</p></td>
</tr>
<tr class="odd">
<td><p>EMAIL FROM</p></td>
<td><p>Displays the valid email address for From line in workflow email.</p>
<p>The default value should be updated at the client site.</p></td>
</tr>
<tr class="even">
<td><p>ENABLED</p></td>
<td><p>If selected, the workflow language message is sent to users in the category.</p>
<p>If disabled, the message is not sent.</p>
<p><strong>NOTE:</strong> The check box is selected by default for all default events with the exception of the LateNotify event.</p>
<p><strong>NOTE:</strong> The LateSummary Event sends a summary email that contains links to Requests that have late roles. The LateNotify event sends individual emails for each late role. If both of these events are enabled, a user receives both a summary email and individual emails for each late Role. It is recommended that either LateNotify Event or LateSummary Event be activated but not both.</p>
<p>Refer to <a href="../Config/Set_Up_SLA_Notifications.htm">Set up SLA Notifications in dspConduct™</a> for more information on SLAs, which  determine when a request is late.</p></td>
</tr>
</tbody>
</table>

## <span id="Category_Workflow_Language_Message_V"></span>Category Workflow Language Message V

[Workflow Language Message H](Category_Workflow_Language_Message_H.htm)

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>EVENT</p></td>
<td><p><em>Displays event that triggers the workflow email to be sent.</em></p>
<p><strong>NOTE:</strong> The name must be unique to the category. The Event name cannot be updated for default events.</p></td>
</tr>
<tr class="odd">
<td><p>SUBJECT</p></td>
<td><p><em>Displays subject line of workflow email.</em>A value preceded and followed by # is a dynamic substitution value for replacement at run time.</p></td>
</tr>
<tr class="even">
<td><p>MESSAGE</p></td>
<td><p><em>Displays body text within the workflow email.</em>A value preceded and followed by # is a dynamic substitution value for replacement at run time.</p></td>
</tr>
<tr class="odd">
<td><p>EMAIL FROM</p></td>
<td><p>Displays valid email address for From line in workflow email.</p>
<p>The default value should be updated at the client site.</p></td>
</tr>
<tr class="even">
<td><p>Attachment</p></td>
<td><p>Displays the fully-qualified name of the file to be attached to the workflow.</p></td>
</tr>
</tbody>
</table>
