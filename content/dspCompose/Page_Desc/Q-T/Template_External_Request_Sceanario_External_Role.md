# Template (External Request Scenario External Role)

<div class="use">

Use this page to [Set External Role Contacts for an External Request
Scenario](../Use_Cases/Set_External_Role_Contacts.htm).

</div>

To access this page:

Select <span style="font-weight: bold;">dspCompose \>
Team</span> from *Navigation *pane.

1.  Click <span style="font-weight: bold;">Templates</span> for a team.
2.  Click <span style="font-weight: bold;">Vertical View</span> for a
    template.
3.  Click <span style="font-weight: bold;">Configuration</span> tab.
4.  Click <span style="font-weight: bold;">External Request
    Scenarios</span>.
5.  Click <span style="font-weight: bold;">External Roles for a
    scenario</span>.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>EXTERNAL ROLE ID</p></td>
<td><p>Displays role assigned to the external contact.</p></td>
</tr>
<tr class="odd">
<td><p>RECIPIENT EMAIL ADDRESS</p></td>
<td><p>Displays email address used for the external contact.</p></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays name of external contact assigned to role. This name is how the user is addressed in the workflow email sent from dspCompose™.</p></td>
</tr>
<tr class="odd">
<td><p>LANGUAGE ID</p></td>
<td><p>Displays language used for external contact workflow emails. If no language is set, English is used as the language.Language-specific messages are added on the Workflow Message page and the Workflow Language Message page</p></td>
</tr>
<tr class="even">
<td><p>USE SENDER EMAIL ADDRESS</p></td>
<td><p>If enabled, the sender of an email to an external role is also the recipient.</p>
<p>Using this process simplifies setting up external contacts for an external request scenario. The current user will:</p>
<ul>
<li>Receive an email from dspCompose™ as a workflow message to initiate the email creation process and</li>
<li>Send email to dspCompose™ when processing the external request scenario for the current request.</li>
</ul>
<p>A validation rule checks to ensure that the Recipient Email Address field is cleared. If disabled, a validation rule checks to ensure that the Recipient Email Address field contains a valid email address.</p></td>
</tr>
</tbody>
</table>
