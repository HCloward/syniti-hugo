# Set a Role's Org Unit Value Assignments

A Security Administrator can include or remove multiple org unit values
at one time for all of the roles in a position . With this option it is
not necessary to configure the org unit values for each individual role
in a position.

Roles are added to categories in dspConduct™ \> Design. Org unit values
differ by category and therefore must be configured separately for each
category included in a position and are applied only to the roles in the
category.

**NOTE:** Category org units become available for security assignment in
a position when the business process assigned to a category is included
the position.

Refer to [Add an Org Unit Type to a Category
Object](Manage_Org_Units.htm#Add_an_Org_Unit_Type_to_a_Category_Object)
and [Add a Role](Add_a_Role.htm) for more information about setting up
org units for a Category and adding roles to a category.

The category org unit value configuration functions as a template for
org unit value assignment to a role in the position. Any role that is
added to the position that belongs to the category for which the org
unit is established is automatically assigned the org unit values that
are included on the *Position Category OrgUnit* page. Any roles that
exist for a position are updated with the org unit values that are
included or removed when the <span style="font-style: italic;">[Position
Category Org Unit](../Page_Desc/Position_Category_Org_Unit1.htm)</span>
page is updated. However, roles can be configured individually if
needed. Refer to <span>[Configure Org Unit Value Assignments for Roles
at the Role
Level](#Configure_Org_Unit_Value_Assignments__at_the_Role_Level) for
more
information.</span>

## <span id="Configure_Org_Unit_Value_Assignments_at_the_Position_Level"></span>Configure Org Unit Value Assignments at the Position Level

Before performing this task, design the governance elements in
dspConduct™ \> Design and add a position. Refer to [dspConduct™ Design
Process Overview](dspConduct_Design_Process_Overview.htm) and [Add a
Position](Add_Position.htm) for more information.

To configure org unit value assignments at the position level:

1.  Select **dspConduct \> Security \> Positions**in the *Navigation*
    pane; the *[Position](../Page_Desc/Position.htm)* page displays.

2.  Click the **Category Org Units** icon; the *[Category Org Units for
    Position](../Page_Desc/Category_Org_Units_for_Position.htm)* page
    displays in the child pane.
    
    *[View the field descriptions for the Category Org Units for
    Position page](../Page_Desc/Category_Org_Units_for_Position.htm)*

3.  Click the **Org Unit1** icon for a **CATEGORY ID.**
    
    *[View the field descriptions for the Position Category OrgUnit1
    page](../Page_Desc/Position_Category_Org_Unit1.htm)*

4.  Select one or more org unit values.

5.  Click the **Include**or **Remove** icon as needed.
    
    The Include All Org Units option allows the user to add all the org
    unit values for all roles within a category that are included in the
    position without having to scroll through the list and select them
    all first.

6.  Repeat steps 3– 5 to add **Org Unit2** and **<span>Org
    Unit3</span>** values as needed.

*<span style="font-size: 12.0pt;">[View the field description for the
Position Category OrgUnit2
page](../Page_Desc/Position_Category_Org_Unit2.htm)</span>*

*<span style="font-size: 12.0pt;">[View the field description for the
Position Category OrgUnit3
page](../Page_Desc/Position_Category_Org_Unit3.htm)</span>*

Next, [configure org unit value assignments for roles at the role
level](#Configure_Org_Unit_Value_Assignments__at_the_Role_Level) if
needed or [configure users in a
position](Configure_Users_in_a_Position.htm).

## <span id="Configure_Org_Unit_Value_Assignments__at_the_Role_Level"></span>Configure Org Unit Value Assignments at the Role Level

Users assigned to a position have access to the data that corresponds to
the org unit values configured for the roles included in the position. A
template for the org unit values that are included or removed for roles
is configured on the[*Category Org Units for
Position*](../Page_Desc/Category_Org_Units_for_Position.htm) page.
Optionally, org unit values to be included or removed for an individual
role can be customized on the *[Position Role Org
Unit](../Page_Desc/Position_Role_Org_Unit_1.htm)* page using the
following steps.

Before performing this task, design the governance elements in
dspConduct™ \> Design and add a position. Refer to [dspConduct™ Design
Process Overview](dspConduct_Design_Process_Overview.htm) and [Add a
Position](Add_Position.htm) for more information.

To configure org unit value assignments for roles at the role level:

1.  Select **dspConduct \> Security \> Positions** in the *Navigation*
    pane.

2.  Click the **Roles** icon for a position.
    
    *[View the field descriptions for the Position Role
    page.](../Page_Desc/Position_Role.htm)*

3.  Click the **Org Unit1** icon.

4.  Click <span style="font-weight: bold;">Add</span>.
    
    *[View the field descriptions for the Position Role Org Unit 1
    page](../Page_Desc/Position_Role_Org_Unit_1.htm).*

5.  Select the org unit value in the **Position Role Org Unit** list
    box.<span> </span>

6.  Click **Save**.

7.  Repeat Steps 3 – 6 to add <span style="font-weight: bold;">Org Unit
    2</span> values and <span style="font-weight: bold;">Org Unit
    3</span> values as needed.

*[View the field descriptions for the Position Role Org Unit 2
page](../Page_Desc/Position_Role_Org_Unit_2.htm).*

*[View the field descriptions for the Position Role Org Unit 3
page](../Page_Desc/Position_Role_Org_Unit_3.htm).*

Next, <span>[configure the read-only/editable settings for org unit
value assignments for
roles](#Configure_the_Read_Only_Editable_setting_for_Org_Unit_Value_Assignments_for_Roles)
if needed or [Configure Users in a
Position](Configure_Users_in_a_Position.htm)</span>.

## <span id="Configure_the_Read_Only_Editable_setting_for_Org_Unit_Value_Assignments_for_Roles"></span>Configure the Read-Only/Editable setting for Org Unit Value Assignments for Roles

For a role, a user has access to the data that corresponds to the org
unit values included in the role. In a position, a System Administrator
can set read only and editable setting, if needed.

If a role is set to read only on the *[Position
Role](../Page_Desc/Position_Role.htm)* page, every org unit value
assigned to the role is set to read only. However, If one of the org
unit values is set to editable on one of the *[Position Role Org
Unit](../Page_Desc/Position_Role_Org_Unit_1.htm)* pages, the role is set
to editable in the position.

The settings control whether or not a user assigned to the position for
this role can edit and take action on the org unit data in the Content
WebApp.

A user can be assigned to multiple positions. The security setup uses
the most permissive setting for users across their assigned positions.
If a user is assigned to two positions, one in which a role has an org
unit value that is set to read only, and one in which a role has the
same org unit set to editable, then the user is considered to have
editable access for that org unit value.

Before performing this task, design the governance elements in
dspConduct™ \> Design and add a position. Refer to [dspConduct™ Design
Process Overview](dspConduct_Design_Process_Overview.htm) and [Add a
Position](Add_Position.htm) for more information.

To configure <span>the read-only or editable setting for org unit value
assignments</span>:

1.  Select **dspConduct \> Security \> Positions** in the *Navigation*
    pane.

2.  Click the **Roles** icon for a position.
    
    *[View the field descriptions for the Position Role
    page](../Page_Desc/Position_Role.htm).*

3.  Click the **Org Unit1,Org Unit2,** or **Org Unit3** icon as needed.

4.  Select one or more org unit values and then click the **Set as Read
    Only** or **Set as Editable** icon as needed.

Next, [configure users in a
position](Configure_Users_in_a_Position.htm).
