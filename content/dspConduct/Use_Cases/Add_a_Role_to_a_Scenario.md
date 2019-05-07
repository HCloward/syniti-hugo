+++
title = 'Add a Role to a Scenario'
solution = 'Master Data Management'
+++

# Add a Role to a Scenario

The [Scenario (Roles)](../Page_Desc/Scenarios_Roles_H.htm) page allows a
Designer to assign one or more roles to a scenario. A role can be added
to multiple scenarios.

Before performing this task, [Create a Category](Create_a_Category.htm)
and [Add a Scenario](Add_Scenario.htm).

To add a role to a scenario in dspConduct™:

1.  Select **dspConduct \> Design** in the *Navigation* pane.

2.  Click the **Scenarios** icon for a category on the *Category* page.

3.  Click the **Roles** icon.
    
    **NOTE**: This icon is disabled if the scenario is not active.

4.  Click **Add**.
    
    [View the field descriptions for the Scenario (Roles)
    page](../Page_Desc/Scenarios_Roles_H.htm)

5.  Select the role ID from the **ROLE ID** list box.

6.  Enter the number of days estimated to complete the tasks assigned to
    the role in the **Work Days** field. (optional)

7.  Enter the number of hours estimated to complete the tasks assigned
    to the role in the **Work Hours** field. (optional)

8.  Enter the number of minutes estimated to complete the tasks assigned
    to the role in the **Work Minutes** field. (optional)
    
    **NOTE**: The Work Days, Work Hours, and Work Minute fields are
    optional. Refer to [Set up SLA notifications in
    dspConduct™](../Config/Set_Up_SLA_Notifications.htm) for more
    information about the prerequisites for setting up SLAs and how the
    SLAs work at the various levels for dspConduct™ elements.

9.  Click **Save**; the *Scenario (Roles)* page’s *Vertical* View
    displays.

10. If this role is an auto post role within the scenario, click the
    **Auto Post Role** check box (optional).
    
    **NOTE**: This option only displays for roles of type Post. If this
    option is enabled, then once the request data dependencies have been
    completed, posting is automatically initiated.

11. If this role is an auto finish role within the scenario, click the
    **Auto Finish Role** check box (optional).

12. If this role has an application role type, click the **Allow Update
    For Extend Scenarios** check box (optional).
    
    **NOTE**: This option is only available for roles of type
    Application assigned to scenarios of type BusinessExtend or
    OrganizationalExtend. At the scenario \> role level this option
    allows the role to update system data within a task that already
    exists in the target. This allows a Designer to control edit
    functionality within the business processes content pages.

13. Click **Save**.

Continue with [Add a Dependent Scenario to a
Scenario](Add_a_Dependent_Scenario.htm).
