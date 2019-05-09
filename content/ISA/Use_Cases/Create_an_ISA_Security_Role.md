## Create an ISA Security Role

A role is a single unit used to authorize specified security to the
assigned user.

The ISA Security Role must be created on site and must have the Collect
Target dgRepository\_IS assigned to the role as a key.

To create the ISA security role in System Administration:

1.  Select <span style="font-weight: bold;">Admin \></span>**Security \>
    Security Definitions \> Security Roles** in *Navigation* pane.

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

9.  Select the name of the IS repository (e.g., Target –
    dgRepository\_IS) from the **SECURITY DEFINITION KEY ID** list box.

10. Click **Save**.

11. Navigate to the *[Security
    Roles](../../../Platform/Sys_Admin/Page_Desc/Security_Roles)*
    page.

12. Click **Web App Groups**.

13. Assign Web App Groups to the security role. Refer to [WebApp
    Groups](../../../Platform/Sys_Admin/Use_Cases/WebApp_Groups) and
    [Assign WebApp Groups to Security
    Roles](../../../Platform/Sys_Admin/Use_Cases/Assign_WebApp_Groups_to_Security_Role)
    for more information.
