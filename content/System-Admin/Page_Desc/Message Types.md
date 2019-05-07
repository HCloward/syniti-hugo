+++
title = 'Message Types H'
solution = 'Platform'
+++

# Message Types H

[Message Types V](#Message)

<div class="use">

Use this page to [Add a Message
Type.](../Use_Cases/Add%20a%20Message%20Type.htm)

</div>

To access this page, select **Admin \> Configuration \> Setup \> Message
Types**.

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
<td><p>Test</p></td>
<td><p>Click to view a sample of the selected message as it displays in the DSP®.</p></td>
</tr>
<tr class="odd">
<td><p>Copy</p></td>
<td><p>Click to copy the message to use as the basis for a new message.</p></td>
</tr>
<tr class="even">
<td><p>MESSAGE TYPE NAME</p></td>
<td><p>Displays the name of the message type.</p>
<p><strong>NOTE</strong>: Use this name when referring to the message type in any custom code.</p>
<p><strong>NOTE</strong>: Name the message so that developers and users can ascertain the scope of the message type and the application it runs in (for example, Cransoft.Event.Error).</p></td>
</tr>
<tr class="odd">
<td><p>TITLE</p></td>
<td><p>Displays the name that displays on the message.</p></td>
</tr>
<tr class="even">
<td><p>IMAGE ID</p></td>
<td><p>Displays the name of the image file used in the message. Images are added on the <em><a href="Images%20H.htm">Images</a></em> page. Refer to <a href="../Use_Cases/Add%20an%20Image%20to%20the%20DSP.htm">Add an Image to the DSP</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>COLOR ID</p></td>
<td><p>Displays the ID for the background color of the message.</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the message.</p>
<p><strong>NOTE</strong>: This can be used to classify the message type as a Notification, Error, or other type.</p></td>
</tr>
<tr class="odd">
<td><p>IMAGE</p></td>
<td><p>Displays the image that is included in the message.</p></td>
</tr>
<tr class="even">
<td><p>COLOR</p></td>
<td><p>Displays the background color of the message.</p></td>
</tr>
</tbody>
</table>

## <span id="Message"></span>Message Types V

[Message Types H](#)

Field

Description

Message Type Name

Displays the name of the message type.

**NOTE**: Use this name when referring to the message type in any custom
code.

**NOTE**: Name the message so that developers and users can ascertain
the scope of the message type and the application it runs in (for
example, Cransoft.Event.Error).

Storage

Retention Days

Displays the number of days the message is stored in the database.

Notification Behavior

Message Expansion Threshold

Displays the maximum number of characters that can display in the
message window.

If the threshold is exceeded, when the message displays to the user, the
message content is replaced with a predefined message, and a link is
provided to view the message content in a separate pane within the DSP. 

Require Action

If checked, the user must click the message to close it.

In unchecked, the message fades after displaying for a few seconds.

Archive

If checked, error messages are archived in the database, and can be
viewed in the Messages tab accessed from the Quick Panel.

Online Alert Only

If checked, if the message is sent when a user is not logged in, it will
not display in the DSP when the user logs in. The user must click the
Messages tab in the Quick Panel to view the message.

If unchecked, the message displays as soon as the user is logged in.

Read On Alert

If checked, when the message displays to the user, it does not increment
the unread message counter displayed on the Messages tab on the Quick
Panel.

If unchecked, the unread message counter is always incremented when a
message with this message type displays.

Workflow Properties

Workflow Send Message

Displays how a workflow message displays in the DSP if this message type
is used with a workflow business rule.

Values are:

  - **Always send**
  - **Never send**
  - **Send only when user is offline**

**NOTE**: If the user is online, the message isn't sent. It doesn't
display in the DSP®, and does not display on the Messages tab in the
Quick Panel.

  - **Send only when user is online**

Refer to [Workflow Views](../Use_Cases/Workflow_Views.htm) for more
information.

Workflow Send Email

Displays how a workflow email is sent to the user if this message type
is used with a workflow business rule.

Values are:

  - **Always send**
  - **Never send**
  - **Send only when user is offline**

**NOTE**: If the user is online, the email isn't sent.

  - **Send only when user is online**

Refer to [Workflow Views](../Use_Cases/Workflow_Views.htm) for more
information.
