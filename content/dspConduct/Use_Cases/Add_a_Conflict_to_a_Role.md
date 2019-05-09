+++
title = 'Add a Conflict to a Role'
solution = 'Master Data Management'
+++

# Add a Conflict to a Role

When a Designer assigns role conflicts, the system does not allow a
single user to execute those same roles within the same request, even if
that user has security to both roles.

Role conflicts help users maintain Sarbanes-Oxley compliance by warning
the security administrator if conflicts of interest exist between a user
and the assigned role(s).

Before this task can be performed, multiple roles must exist within the
category.<span> </span>Refer to [Add a Role](Add_a_Role) for more
information.

To add conflicts to roles:

1.  Select <span style="font-weight: bold;">dspConduct \>
    </span>**Design** in the *Navigation* pane.

2.  Click the **Roles** icon for a category.

3.  Click the **Conflicts** icon for a role.

4.  If no conflicts exist, the page displays in add mode. Otherwise
    click **Add**.
    
    [View the field descriptions for the Role (Conflicts)
    page.](../Page_Desc/Role_Conflicts)

5.  Select the name of the role that is in conflict with the role
    selected on the
    <span style="font-style: italic;">[Role](../Page_Desc/Role_H_dspConduct)</span>
    page from the **CONFLICTROLEID** list box.
    
    **NOTE:** A user who is assigned to both roles can only execute one
    during the request posting process.

6.  Click **Save**; <span style="font-style: italic;">Vertical</span>
    View displays.

7.  Enter information as to why the roles are in conflict in the
    **Comment** field, if needed.

8.  Click <span style="font-weight: bold;">Save</span>.
