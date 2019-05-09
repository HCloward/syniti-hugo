+++
title = 'Create a User Account Based on Another User’s Security Settings'
solution = 'Platform'
+++

# Create a User Account Based on Another User’s Security Settings

An Administrator can use the Create User From option on the
<span style="font-style: italic;">[Users](../Page_Desc/Users_H)</span>
page to copy a user’s WebApp permissions and security roles to use as
the basis for configuring security settings when creating a new user
account.

When copying the settings, an Administrator can update them by changing
permissions to access WebApps and WebApp groups or by setting an
expiration date for assignment to a WebApp group. Setting an expiration
date may be useful when a user must perform another user’s tasks for a
limited time. When the expiration date has passed, the user no longer
has access to the WebApp group.

Refer to [WebApp Groups](WebApp_Groups) and [Add Users to WebApp
Groups](Assign_Users_to_WebApp_Groups) for general information.

To create a user and copy the security settings from another user’s
account:

1.  Select
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Admin
    \> Security \> Users</span> in the
    <span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">Navigation</span>
    pane.

2.  Select a user to copy.

3.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Create
    User From</span> icon.

4.  Click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Edit</span>.:
    
    *[View the field descriptions for the Copy User
    page](../Page_Desc/Copy_User)*

5.  Enter a user name in the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">User
    ID</span> field.
    
    **NOTE**: The user uses this ID to log in to the Platform.

6.  Enter a name in the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Name</span>
    field.

7.  Enter a password in the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Password</span>
    field.
    
    **NOTE**: The encrypted password displays as asterisks. To view the
    password, click the icon in the field.
    
    **NOTE**: Password configuration determines valid passwords. Refer
    to [Configure Password Options](Configure_Password_Options) for
    more information.

8.  Enter the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Windows
    Username</span> for the user, if using Integrated authentication.

9.  Enter the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">email
    address</span> for the user.

10. Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Copy
    Security Roles</span> check box if needed..
    
    **NOTE:** It is enabled by default. If the security roles are not to
    be copied, disable the field.

11. Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Permissions</span>
    icon to update permissions to individual WebApps and WebApp Groups,
    or to set an expiration date for assignment to a WebApp group, if
    needed. See the steps below for additional information.

12. Click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Save</span>.

13. Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Create</span>
    icon on the Page toolbar; the new user displays on the
    <span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">Users</span>
    page.

While creating a user based on another user's security settings, an
Administrator can update security settings.

To exclude the user from a WebApp:

1.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Permissions</span>
    icon on the
    <span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">Copy
    User</span> page.
2.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Revoke
    Web App Access</span> button.

To exclude the user from a WebApp group:

1.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Permissions</span>
    icon on the
    <span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">Copy
    User</span> page.

2.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Groups</span>
    icon.

3.  Click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Edit</span>.
    
    [View the field descriptions for the Copy WebAppGroupUser
    page.](../Page_Desc/Copy_WebAppGroupUser)

4.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Exclude</span>
    check box to enable it to revoke the user’s permissions to access
    pages that are assigned to the WebApp group.

To set an expiration date for a user’s access to a WebApp group:

1.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Permissions</span>
    icon on the
    <span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">Copy
    User</span> page.

2.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Groups</span>
    icon.

3.  Click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Edit</span>.
    
    [View the field descriptions for the Copy WebAppGroupUser
    page.](../Page_Desc/Copy_WebAppGroupUser)

4.  Click in the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">EXPIRATION
    DATE </span>field and enter the date when a user should no longer
    have access to the pages associated with the WebApp group.

5.  Click
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Save</span>.
