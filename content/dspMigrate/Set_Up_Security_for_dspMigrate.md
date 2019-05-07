+++
title = 'Set Up Security for dspMigrate™ Advanced Data Migration (ADM)'
solution = 'Migration'
+++

# Set Up Security for dspMigrate™ Advanced Data Migration (ADM)

To set up security for dspMigrate™ Advanced Data Migration (ADM)an
Administrator:

1.  [Creates User
    Accounts](../../Platform/Sys_Admin/Use_Cases/Create_User_Accounts_in_System_Administration.htm)
2.  [Creates Security
    Roles](../../Platform/Sys_Admin/Use_Cases/Define_Security_Roles1.htm)
3.  [Assigns Users to Security
    Roles](../../Platform/Sys_Admin/Use_Cases/Assign_Users_to_Security_Roles.htm)
4.  [Assigns WebApp Groups to Security
    Roles](../../Platform/Sys_Admin/Use_Cases/Assign_WebApp_Groups_to_Security_Role.htm)

**NOTE:** The security roles needed for a migration project are subject
to project team organization, structure and assign the work. For
example, if a new role called FieldMapper is created for Map, the
assigned security roles WebApp ID/Group ID may look like the following:
CranSoft/User, CranPort/User, Console/User and Map/Field Mapper.

<span style="font-weight: bold;">NOTE:</span> The Migration Developer
security role is installed with the platform. Users assigned to this
security role have access to all Waves, Process Areas, objects, targets
and sources as well as Transform and AutoGen. The Administrator user is
added to this security group by default, but other users can be added.

5.  Set up Waves, Process Areas, and objects in Console and Targets and
    Sources in Target Design. Refer to [Create the Contexts for
    Migration
    Projects](../Console/Use_Cases/Create_Contexts_for_Migration_Projects.htm),
    [Add a
    Target](../Design/Use_Cases/Add_a_Target_in_Target_Design.htm) and
    [Add a Source](../Design/Use_Cases/Assign_a_Source_to_a_Target.htm)
    for more information.

<!-- end list -->

6.  An Administrator must [assign keys to security
    roles](../../Platform/Sys_Admin/Use_Cases/Assign_Keys_to_Security_Role.htm)
    for all levels of the hierarchy, which are the following:

<!-- end list -->

  - Wave-Process Area combination
  - Wave-Process Area-Object combination
  - Wave-Process Area-Object-Target combination
  - Wave-Process Area-Object-Target-Source combination

**NOTE**: If a user is not assigned to the Migration Developer security
role, security keys must be assigned to that user's role every time a
new hierarchy is created in Console and Target Design.

An Administrator can also [Set the Default Context for a
User](../../Platform/Sys_Admin/Use_Cases/Set_the_Default_Context_for_a_User.htm).
