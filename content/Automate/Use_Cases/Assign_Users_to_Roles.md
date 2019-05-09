+++
title = 'Assign Users to Roles'
solution = 'Platform'
+++

# Assign Users to Roles

Assign users to roles so that specific users can receive the appropriate
notifications. The “Best Practice” is to add the From Email to the Admin
group and make two or more groups of users assigned to the Development
and Business roles.

**NOTE:** Users are added in System Administration. Refer to [Getting
Started with DSP Security for Delivered
Components](../../Sys_Admin/Use_Cases/GettingStartedwDSPSecurityDlvrdComps)
for more information.

To assign users to a role in Automate:

1.  Select **Configuration \> Roles** in the *Navigation* pane.

2.  Click the **Users** icon for the desired role.

3.  Click **Add**.
    
    [View the field description for the Role (Instance)
    page](../Page_Desc/Role_Instance)

4.  Select an instance from the **INSTANCE** list box.
    
    **NOTE:** The Instance selected MUST match the Instance field in 2
    additional places in order for email notifications to properly work:
    the *[Parameters](../Page_Desc/Parameters)* page in Automate and
    the
    *[Parameters](../../Sys_Admin/Page_Desc/Parameters_All_TabsSysAdmin)*
    page in System Administration.

5.  Select a user ID from the **USER ID** list box.

6.  Click **Save**.
