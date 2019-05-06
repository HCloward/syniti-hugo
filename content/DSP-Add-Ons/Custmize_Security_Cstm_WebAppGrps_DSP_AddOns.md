## Customize Security with Custom WebApp Groups Using DSP Add-Ons

An Administrator can use DSP Add-Ons to create custom security for
delivered WebApps or custom WebApps. By creating Custom WebApp groups,
users can easily customize access for pages depending on any
organizational need. For example, WebApp groups could be created for
departments, to group pages that are used to perform certain tasks, or
to grant access to a page to a limited number of users.

**NOTE**: To access DSP Add-Ons, the user must be logged in with the
Administrator account.

To customize security with DSP Add-Ons at a high level:

1.  Add a WebApp group to a component.

2.  Add pages from the component to the WebApp group.
    
    **NOTE**: The ability to view, add, update or delete records on a
    page can also be set for a WebApp group.

3.  Assign security roles to the WebApp group.

4.  Assign users to the security role who should access the pages using
    the WebApp group.
    
    **NOTE**: WebApp groups must be published before they can be used by
    the platform.

To customize security:

1.  Click **DSP Add-Ons** in the *Navigation* pane.

2.  Click **Web App Groups** for a WebApp.
    
    **NOTE**: If no records exist, the page displays in add mode.
    Otherwise, click Add.
    
    *[View the field descriptions for the Groups
    page.](Groups_DSP_AddOns.htm)*

3.  Enter a descriptive name in the **GROUP NAME** field.
    
    **NOTE**: This could be the name of a department, such as Sales or
    HR.

4.  Click **Save**.

5.  Click **Pages**.
    
    <span style="font-weight: bold;">NOTE</span>: If no records exist,
    the page displays in add mode. Otherwise, click Add.
    
    *[View the field descriptions for the Group Pages
    page.](Group_Pages_DSP%20Add%20Ons.htm)*

6.  Select the name of the page in the selected component that should be
    assigned to the WebApp group from the **PAGE ID** list box.
    
    **NOTE**: By default, security access is set to allow all
    functionality associated with the page. To remove access to certain
    functionality for the user who will be assigned to this WebApp group
    through a security role, disable the check boxes as needed.

7.  Click **Save**.
    
    **NOTE**: The page remains in add mode to simplify adding multiple
    pages to the WebApp group. When all pages have been added, click
    **Cancel**.

8.  Click **Security Roles** on the *Groups* page.
    
    **NOTE**: If no records exist, the page displays in add mode.
    Otherwise, click **Add**.
    
    *[View the field descriptions for the Security Roles
    page.](Security_Roles_\(DSP_Add-Ons\).htm)*

9.  Select the security role from the **ROLE ID** list box.
    
    **NOTE**: Security roles installed with the platform and custom
    security roles display. Refer to [Create Security
    Roles](../Sys_Admin/Use_Cases/Create_Security_Roles.htm) for more
    information.
    
    **NOTE**: The page remains in add mode to simplify adding multiple
    security roles to the WebApp group. When all roles have been added,
    click **Cancel**.

10. Click **Publish To Framework** on the *Groups* page. The WebApp
    group is then assigned to the security role, and all users assigned
    to that security role can access the pages in that WebApp group.

11. Assign users who should access the pages using the WebApp group to
    the security role. Refer to [Assign Users to Security
    Roles](../Sys_Admin/Use_Cases/Assign_Users_to_Security_Roles.htm)
    for more information.
    
    **NOTE**: These WebApp groups will then be active, and the users
    assigned to the security roles will access the pages as determined
    by the WebApp group settings.
    
    **NOTE**: Custom WebApp groups created with DSP Add-Ons can be
    republished to the framework if changes are made. When upgrading the
    platform during an installation, these WebApp groups will not be
    overwritten and can be published to the framework again after the
    upgrade.
