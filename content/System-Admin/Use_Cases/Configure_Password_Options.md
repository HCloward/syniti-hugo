+++
title = 'Configure Password Options'
solution = 'Platform'
+++

# Configure Password Options

An Administrator can set restrictions on passwords.

<span style="font-weight: bold;">NOTE</span>: Changes made to password
settings affect passwords that are added and updated after the settings
have been updated. Passwords created before the settings were updated
are not affected.

<span style="font-weight: bold;">NOTE</span>: An Administrator can also
prevent users from updating their passwords to specific words or
numbers, e.g., “1234” or “password.” Refer to [Set Forbidden
Passwords](Set_Forbidden_Passwords.htm) for more information.

The following settings are available on the
<span style="font-style: italic;">[Parameters](../Page_Desc/Parameters_All_TabsSysAdmin.htm)</span>
page Security Settings tab.

  - **Maximum Password Age -**
    <span style="font-family: Arial, sans-serif;">Sets the number of
    days before user account passwords expire. Once expired, users are
    required to reset their password. Enter 0 for the password to never
    expire. Default value is 30 days.</span>
  - **Min Password Length -**
    <span style="font-family: Arial, sans-serif;">Sets the minimum
    password length for new or changed passwords. Zero allows any
    password length. Default value is 0.</span>
  - **Password Require Alpha -**
    <span style="font-family: Arial, sans-serif;color: #000000;">Sets
    the requirement that users' passwords must contain at least one
    alpha character (A-Z or a-z).</span>
  - **Password Require Numeric -**
    <span style="font-family: Arial, sans-serif;color: #000000;">Sets
    the requirement that users' passwords must contain at least one
    numeric character (0-9).</span>
  - **Password Require Special -**
    <span style="font-size: 11.0pt;line-height: 107%;font-family: Arial, sans-serif;">Sets
    the requirement that users' passwords must contain at least one
    special character (e.g., ? \# \! @ $ %).</span>
  - **Password History -**
    <span style="font-family: Arial, sans-serif;">Sets the number of
    passwords retained for each user. When a user sets a new password,
    the platform compares that password with the previous passwords to
    prevent password reuse. For example, if the Password History setting
    is 6, the Platform compares a password reset with that user’s 6
    previous passwords and does not allow the user to enter a duplicate.
    A setting of 0 retains no passwords except the current one (i.e.,
    there is no check for unique passwords for a user). Default value is
    0.</span>
