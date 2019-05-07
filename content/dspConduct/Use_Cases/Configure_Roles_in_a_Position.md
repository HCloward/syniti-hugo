+++
title = 'Configure Roles in a Position'
solution = 'Master Data Management'
+++

# Configure Roles in a Position

A Security Administrator can include or remove roles to a position.
Before performing this task, design the governance elements in
dspConduct™ \> Design and add a position. Refer to [dspConduct™ Design
Process Overview](dspConduct_Design_Process_Overview.htm) and [Add a
Position](Add_Position.htm) for more information.

Roles can have conflicts where the same user is not allowed to finish
both roles within a conflicting role pair. A user cannot be included in
position(s) with roles that are designed to conflict on the
[<span style="font-style: italic;">Role
(Conflicts)</span>](../Page_Desc/Role_Conflicts.htm) page in dspConduct™
\> Design. Refer to [Add a Conflict to a
Role](Add_a_Conflict_to_a_Role.htm) for more information.

To configure roles in a position in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \>
    </span>**Security \> Positions** in the *Navigation* pane.

2.  Click the **Roles** icon for a position.
    
    *[View the field descriptions for the Position Role
    page](../Page_Desc/Position_Role.htm).*

3.  Select one or more roles, and then click the **Include** or
    **Remove** icon as needed.
    
    The Include All Roles option allows the user to include all of the
    roles in the position without having to scroll through the list and
    select them all first.
    
    <span style="font-weight: bold;">NOTE:</span> If a role is removed
    from a position that has role level org unit value assignments, all
    of the org unit value assignments are removed from the role on the
    <span style="font-style: italic;">[Position
    Role](../Page_Desc/Position_Role.htm)</span> page. If the role is
    later included in the position, the org unit value assignments must
    be recreated.
    
    <span style="font-weight: bold;">NOTE:</span> This option allows a
    System Administrator to set the Read Only/Editable setting for all
    of the org unit values for a role.  If a role is set to read only,
    every org unit value assigned to the role is set to read only.
    However, this setting can be overwritten at the org unit value
    level.  If  any one of the org unit values is set to editable on the
    Position Role Org Unit 1 2 or 3 page, the role is editable. Refer to
    [Configure the Read-Only/Editable setting for Org Unit Value
    Assignments](Set_a_Roles_Org_Unit_Value_Assignments.htm#Configure_the_Read_Only_Editable_setting_for_Org_Unit_Value_Assignments_for_Roles)
    for Roles for more information.

Next, [Set a Role's Org Unit Value
Assignment](Set_a_Roles_Org_Unit_Value_Assignments.htm#Configure_Org_Unit_Value_Assignments_at_the_Position_Level).
