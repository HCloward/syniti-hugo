# 

## Configure ISA Security if the dgRepository\_IS does not display as a Target in Collect

If security is not configured properly, the dgRepository\_IS will not
display on the *Targets* page in Collect. The *Targets* page is used to
refresh the tables in the database, and this task can’t be performed if
the dgRepository\_IS database is not available.

The dgRepository\_IS database in installed with the product but may not
visible to the user because of the user’s security settings.

To make the database accessible to refresh the tables on the *Targets*
page in Collect, set up a security role for the ISA.

A role is a single unit used to authorize specified security to the
assigned user.

The ISA Security Role must be created on site.

To create the ISA security role:

1.  Select <span style="font-size: 11.0pt;font-weight: bold;">Admin
    \></span> **Security \> Security Definitions \> Security Roles** in
    *Navigation* pane.

2.  Click **Add**.
    
    *[View the field descriptions for the Security Roles
    page](../../../Platform/Sys_Admin/Page_Desc/Security_Roles)*

3.  Enter a unique name of the role, such as ISA, in the **NAME** field.

4.  Enter a brief description or explanation of the role in
    **DESCRIPTION** field.

5.  Click **Save**.

6.  Click **Keys**.

7.  Click **Keys** for Collect Targets.

8.  Click **Edit**.
    
    *[View the field descriptions for the Role Key Values
    page.](../../../Platform/Sys_Admin/Page_Desc/Role_Key_Values)*

9.  Select the name of the IS repository (i.e., Target –
    dgRepository\_IS) from the **SECURITY DEFINITION KEY ID** list box.

10. Click **Save.**

11. Navigate to the *[Security
    Roles](../../../Platform/Sys_Admin/Page_Desc/Security_Roles)*
    page.

12. Add the user who should access the database to refresh it in Collect
    to the ISA Security role. Refer to [Assign Users to Security
    Roles](../../../Platform/Sys_Admin/Use_Cases/Assign_Users_to_Security_Roles)
    for more information.
