+++
title = 'Create a User Account in Common'
solution = 'Platform'
+++

# Create a User Account in Common

New users often need to be added to the system. An Administrator creates
user accounts as the first step in the security setup process. Using
Excel Integration on the *[User
Management](../Page_Desc/User_Management_H.htm)* page, an Administrator
can add and update user account data for multiple accounts at one time.
If using Excel Integration, the steps in this topic do not apply.
However, the Administrator will still need to [send the new users a
temporary password](Send_a_Temporary_Password_to_a_User.htm) once the
spreadsheet has been imported.

All fields required for user maintenance are available in the Excel
spreadsheet downloaded from the *User Management* page, though some of
these fields do not display on the *User Management* page’s *Horizontal*
View.

Refer to [Use Excel
Integration](../../Excel_Int/Use_Excel_Integration.htm) for more
information.

**NOTE:** A user who belongs to the UserManager WebApp Group in Common
can add users across the DSP®  , but cannot grant users access to
dspConduct™. A user must also belong to the UserManager WebApp Group in
dspConduct to add dspConduct users. These users can then be added on the
[User
Position](../../../Master_Data_Mgmt/dspConduct/Page_Desc/User_Position.htm)
page. Refer to [Configure dspConduct Positions for a
User](../../../Master_Data_Mgmt/dspConduct/Use_Cases/Configure_dspConduct_Positions_for_a_User.htm)
for more information. For more information regarding WebApp groups,
refer to the following topics in System Administration:

  - [WebApp Groups](../../Sys_Admin/Page_Desc/WebApp_Groups_H.htm)
  - [Create WebApp
    Groups](../../Sys_Admin/Use_Cases/Create_WebApp_Groups.htm)

To create a user:

1.  Select **Common \> User Management** in the *Navigation* pane.

2.  Click **Add.**
    
    [View the field description for the User Management
    page](../Page_Desc/User_Management_H.htm)

3.  Enter a unique ID to be used when logging in to DSP® in the **USER
    ID** field.

4.  Enter the user’s first and last name in the **NAME** field.
    
    **NOTE:** If the **NAME** entered already exists, the user will be
    prompted with a message as to whether or not to accept the
    duplication. If the duplication is accepted, the record is not
    validated.

5.  Enter an **E MAIL Address.**

6.  Select a value from the **LANGUAGE ID** list box.

7.  Select the calendar for the user from the **CALENDAR ID** list box.
    
    **NOTE:** Refer to [Use a Calendar](Use_a_Calendar.htm) for more
    information about setting up calendars.

8.  Click **Save.**:
    
    **NOTE:** The new user is also added to the
    *[Users](../../Sys_Admin/Page_Desc/Users_H.htm)* page in System
    Administration.

Proceed with [Send a Temporary Password to a New
User](../Page_Desc/Results.htm).
