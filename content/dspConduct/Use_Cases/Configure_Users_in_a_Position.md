# Configure Users in a Position

A Security Administrator can add users to a position. Before performing
this task a user account must be created and configured in Common. Refer
to [Create User Accounts in
Common](../../../Platform/Common/Use_Cases/Create_User_Accounts_in_Common.htm)
for more information. An Administrator can also create user accounts.

Common’s *[User
Management](../../../Platform/Common/Page_Desc/User_Management_H.htm)*
page, where user accounts are created and configured, can be accessed in
dspConduct™ by selecting **dspConduct \> Security \> Common: User
Management** in the *Navigation* pane.  

<span style="font-weight: bold;">NOTE:</span> Adding a user in Common
allows for a more streamlined process for password maintenance, and is
the recommended method for use by a Help Desk or Call Center. In Common,
password maintenance is the user’s responsibility. In System
Administration, the Administrator must add a password for the user.
Aside from password maintenance, after the user account is created,
there is no difference between a user account added in Common or System
Administration.

<span style="font-weight: bold;">NOTE</span>: A user must belong to the
Users Manager WebApp Group in dspConduct™ to configure security for
dspConduct™ users. An Administrator adds users to WebApp Groups.

<span style="font-weight: bold;">NOTE:</span> A user can be assigned to
multiple positions. The security setup uses the most permissive setting
for users across their assigned positions. If a user is assigned to two
positions, one in which a role has an org unit value that is set to read
only, and one in which a role has the same org unit set to editable,
then the user is considered to have editable access for that org unit
value.

<span style="font-weight: bold;">NOTE:</span> All users in a position
must be assigned to the same calendar in Common. Refer to [Use a
Calendar](../../../Platform/Common/Use_Cases/Use_a_Calendar.htm) for
more information.

When including users in a position, role conflicts are applied based on
the roles that have been added to the position, and the role conflicts
established on the *[Role (Conflicts)](../Page_Desc/Role_Conflicts.htm)*
page. Refer to [Add a Conflict to a Role](Add_a_Conflict_to_a_Role.htm)
for more information.

To configure users in a position in dspConduct™:

1.  Select **dspConduct \> Security \> Positions** in the *Navigation*
    pane.

2.  Click the **Users** icon for a position.
    
    *[View the field descriptions for the Position User
    page](../Page_Desc/Position_User.htm).*

3.  Select a user, and then click the **Assign Calendar** icon to open
    the *[User
    Management](../../../Platform/Common/Page_Desc/User_Management_H.htm)*
    page to assign a calendar to the user.
    
    **NOTE:** A user must have a calendar assigned to be included in a
    position.

4.  Navigate back to the *User Position* page .

5.  Select one or more users, and then click the **Include** or
    **Remove** icon as needed.
