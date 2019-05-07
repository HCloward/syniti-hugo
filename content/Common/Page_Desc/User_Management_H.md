+++
title = 'User Management H'
solution = 'Platform'
+++

# User Management H

[User Management V](#User_Management_V)

<div class="use">

Use this page to:

  - [Create a User Account in Common](../Use_Cases/Create_a_User.htm)
  - [Send a Temporary Password to a New
    User](../Use_Cases/Send_a_Temporary_Password_to_a_User.htm)
  - [Reset a User's
    Password](../Use_Cases/Reset%20a%20User's%20Password.htm)
  - [Assign an Expiration Date to a
    User](../Use_Cases/Assign_an_Expiration_Date_to_a_User.htm)

</div>

To access this page, select **Common \> User Management** in the
*Navigation* pane.

<span style="font-weight: bold;">NOTE:</span> Excel Integration has been
enabled on this page to allow for Excel-driven user management. Refer to
[Use Excel Integration](../../Excel_Int/Use_Excel_Integration.htm) and
the Knowledge Base article [Use Excel Integration to Create or Update
Multiple User
Accounts](https://support.boaweb.com/hc/en-us/articles/115015883247--DSP-Administration-Use-Excel-Integration-to-Create-or-Update-Multiple-User-Accounts)
for more information.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Set Password and Notify User</p></td>
<td><p>Click to send the “user creation email” to a newly created user that has not logged in. This email is sent only the first time. When this icon is clicked for an existing user that has previously logged in, the user receives a “password reset” email. Both emails contain a temporary password and a link to log into the system. At which time, the user is prompted to change the password.</p>
<p>Refer to the <a href="Parameters_User_Management.htm">Parameters - User Management</a> page for more information about the content of the email sent to the user.</p>
<p><strong>NOTE:</strong> The Set Password and Notify User icon is disabled for users with security set through Windows Authentication.</p></td>
</tr>
<tr class="odd">
<td><p>Security Roles</p></td>
<td><p>Click to open the <a href="User_Role.htm">User Role</a> page to assign a user to a security role. Security roles drive user security and are assigned to users at the role level.</p>
<p>Security roles can also be defined by an Administrator.</p>
<p><strong>NOTE:</strong> Assigning roles to users using either method (Common or System Administration) produces the same results.</p></td>
</tr>
<tr class="even">
<td><p>dspConduct™ Positions</p></td>
<td><p>Click to open the <em>User Settings</em> page in the parent pane and the <a href="../../../Master_Data_Mgmt/dspConduct/Page_Desc/User_Position.htm">User Position</a> page in the child pane.</p>
<p>The <span style="font-style: italic;">User Settings</span> page allows an Administrator to set workflow notification options for a user. Refer to <a href="../../../Master_Data_Mgmt/dspConduct/Config/Set_User_Workflow_Receipt_Preferences.htm">Set User Workflow Receipt Preferences</a> for more information.</p>
<p>The <span style="font-style: italic;"><a href="../../../Master_Data_Mgmt/dspConduct/Page_Desc/User_Position.htm">User Position</a></span> page allows the Administrator to configure dspConduct™ positions to which a user has access. Refer to <a href="../../../Master_Data_Mgmt/dspConduct/Use_Cases/Configure_dspConduct_Positions_for_a_User.htm">Configure dspConduct™ Positions for a User</a> for more information.</p>
<p>If the selected user does not have access to dspConduct™, the icon is disabled. Once the user is added to a role that has access, the icon is  active.</p>
<p>If the user that is logged in does not have access to dspConduct™, the icon is not displayed.</p></td>
</tr>
<tr class="odd">
<td><p>USER ID</p></td>
<td><p>Displays ID associated with user used to log in to the Platform.</p></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the name of user associated with the User ID.</p></td>
</tr>
<tr class="odd">
<td><p>E-MAIL ADDRESS</p></td>
<td><p>Displays the email address of the user associated with the User ID. This email address is used for all workflow notifications.</p></td>
</tr>
<tr class="even">
<td><p>LANGUAGE ID</p></td>
<td><p>Displays the language used for the user’s session.</p></td>
</tr>
<tr class="odd">
<td><p>CALENDAR ID</p></td>
<td><p>Displays the calendar assigned to the user. Refer to <a href="../Use_Cases/Use_a_Calendar.htm">Use a Calendar</a> in Common for more information about setting up calendars.</p></td>
</tr>
</tbody>
</table>

## <span id="User_Management_V"></span>User Management V

[User Management H](#User_Management_H)

<div class="use">

Use this page to [Send a Temporary Password to a
User](../Use_Cases/Send_a_Temporary_Password_to_a_User.htm).

</div>

Field

Description

User Id

Displays ID associated with user used to log in to the Platform.

Name

Displays name of user associated with the User ID.

Security Information

Windows User Name

Displays the login name used for Microsoft Windows to log in to the
Platform. This field is used if Integrated Authentication is enabled to
validate against the Windows domain.

Expiration Date

Displays date when the user’s access to the DSP® will be terminated. If
blank, the user’s access will not expire.

Anonymous

If enabled, the user is an anonymous user. An anonymous user does not
log in to the Platform, but is navigated directly to a specific Platform
page via a workflow link.

Resend User Creation EMail

Click to resend the new user creation email for the selected user. This
happens for a new user who has not logged into the system or an existing
user who has logged into the system. The email contains the user name
and a temporary password

Refer to the [Parameters - User
Management](Parameters_User_Management.htm) page for more information
about the content of the email sent to the user.

**NOTE:** The Resend User Creation Email icon is disabled for users with
security set through Windows Authentication.

Defaults

Language ID

Displays the language used for the user’s session.

Default Page ID

Displays page that opens when the user first logs in to the Platform.
The default value is the Platform Site page.

Style ID

Displays style used within the DSP® for the logged in user. The style
controls colors, fonts, etc. of the user interface.

Calendar ID

Displays the calendar assigned to the user. Refer to [Use a
Calendar](../Use_Cases/Use_a_Calendar.htm) for more information about
setting up calendars.

Contact Information

Telephone

Displays the phone number of the selected user.

Telephone Extension

Displays the telephone extension of the selected user.

E-Mail Address

Displays the email address of the user associated with the User ID. This
email address is used for all workflow notifications.

Format Options

Locale ID

Displays the locale used to translate date and number formats for the
user.

Logs

View Log In History

This icon is not used.
