# Workflow Log H

[Workflow Log V](#Workflow_Log_V)

<div class="use">

Use this page to [View the Workflow
Log](../Use_Cases/View%20the%20Workflow%20Log.htm).

</div>

To access this page, select **Admin \> Resources \> Workflow Log**.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>SUBJECT</p></td>
<td><p>Displays the subject of the email.</p></td>
</tr>
<tr class="odd">
<td><p>TO RECIPIENTS</p></td>
<td><p>Displays the email address of the user who received the email, if the email was sent successfully.</p></td>
</tr>
<tr class="even">
<td><p>ISSUED DATE</p></td>
<td><p>Displays the date and time the email was sent.</p></td>
</tr>
<tr class="odd">
<td><p>WEB APP ID</p></td>
<td><p>Displays the name of the WebApp associated with the workflow.</p></td>
</tr>
<tr class="even">
<td><p>PAGE ID</p></td>
<td><p>Displays the name of the service page In the WebApp that sent the email.</p></td>
</tr>
<tr class="odd">
<td><p>FAILED TO SEND EMAIL</p></td>
<td><p>If enabled, the email was not sent.</p>
<p><strong>NOTE:</strong> Error messages display on the <em>Vertical</em> View.</p>
<p><strong>NOTE:</strong> The Workflow Continue on Error setting set on the <em><a href="Parameters_All_TabsSysAdmin.htm">Parameters</a></em> page determines if the Platform fails events due to SMTP errors that occur when sending workflows. If this setting is enabled, SMTP errors do not prevent the workflow from continuing to process.</p></td>
</tr>
</tbody>
</table>

[](#)

## Workflow Log V

[Workflow Log H](#)

This page contains the following tabs:

  - [General](#General)
  - [Recipients](#Recipients)
  - [Email
Attachments](#Email_Attachments)

### <span id="General"></span>General

|                                    |                                                                                 |
| ---------------------------------- | ------------------------------------------------------------------------------- |
| Field                              | Description                                                                     |
| Web App ID                         | Displays the name of the WebApp associated with the workflow.                   |
| Page ID                            | Displays the name of the service page In the WebApp that sent the email.        |
| Event                              | Displays the type of event that ran that resulted in the workflow being sent.   |
| Issuer User ID                     | Displays process.                                                               |
| Issued Date                        | Displays the date and time the email was sent.                                  |
| Subject                            | Displays the subject of the email.                                              |
| Time to Send Email in Milliseconds | Displays the amount of time it took for the process that sent the email to run. |
| Mail Server Address                | Displays the address of the email server that sent the email.                   |
| Error Messages                     | Displays error messages sent by the email server if the email failed to send.   |

### <span id="Recipients"></span>Recipients

|                 |                                                                                                                                           |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| Field           | Description                                                                                                                               |
| To Recipients   | Displays the user(s) in the To line of the email.                                                                                         |
| CC Recipients   | Displays the user(s) who were CC’ed on the email.                                                                                         |
| BCC Recipients  | Displays the user(s) who were BCC’ed on the email.                                                                                        |
| From Recipients | Displays the user(s) in the From line of the email. For some delivered components, this address may be configured at the component level. |

### <span id="Email_Attachments"></span>Email Attachments

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Email Attachment Count</p></td>
<td><p>Displays the number of files attached to the email.</p></td>
</tr>
<tr class="odd">
<td><p>Total Email Attachment Size in Bytes</p></td>
<td><p>Displays the file size of the email.</p>
<p><strong>NOTE:</strong> The Maximum Email Attachment File Size, set on the <a href="Parameters_All_TabsSysAdmin.htm">Parameters</a> page, sets the file size limit. If the attachment file size exceeds this limit, the email is sent but the workflow is not attached.</p></td>
</tr>
</tbody>
</table>
