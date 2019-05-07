+++
title = 'Manage Org Units'
solution = 'Data Quality'
+++

# Manage Org Units

Org Units are defined at the object level and then added to a category.
Org units are used to create requests for posting to one or many target
systems and define security access to data for users.

Org Units are optional and used to set request data security by
restricting data a user can access based on, for example, an
organization’s structure. A Designer could create an org unit called
Plant that contains the org unit values for plants in different states.
Users can be assigned to the plant in their state, and those users only
see data associated with that org unit value (i.e., the state name).
Additionally a Designer could configure one set of validations, one set
of dependencies and configuration options based on Org Units.

An advanced user, usually a BackOffice Consultant, could implement this
feature to restrict list box values, to limit access to a role during
the request process, or to set role dependencies.

To work with org units:

  - [Add Org Units](#Add_Org_Units)
  - [Add an Org Unit Type to a Category
    Object](#Add_an_Org_Unit_Type_to_a_Category_Object)
  - [Add and Configure Org Unit Groups, Types and
    Values](#Add_and_Configure_Org_Unit_Groups,_Types,_and_Values)

## <span id="Add_Org_Units"></span>Add Org Units

This task is performed by a Designer.

Before performing this task, Org Unit source tables must exist in a
content database. The source tables are used as Org Unit list sources in
dspConduct™ configuration, so that the Org Units can be applied as Org
Unit Types within each category. There is no restriction to the number
or type of Org Units that may be configured.

All Org Units are global, defined at the configuration level and used
across categories. Once added, an Org Unit record cannot be edited. If
changes need to be made to an Org Unit, delete the record and add a new
Org Unit.

The *Org Units* page is used to register lists (source tables) that
reside in any content database.

<span style="font-weight: bold;">NOTE:</span> Org Units are an optional
feature.

To add organizational units:

1.  Select <span style="font-weight: bold;">dspConduct </span>**\>
    Configuration \> Org Units** in the *Navigation* pane.

2.  If no records exist, the page displays in add mode. Otherwise, click
    **Add**.
    
    *<span style="color: #0000ff;">[View the field descriptions for the
    Org Units page](../Page_Desc/Org_Units.htm)</span>*

3.  Enter a unique name in the **ORG UNIT** field.
    
    **NOTE:** This name describes the Org Unit, such as Plant or
    Company. It can contain all letters, 0-9 and underscores only.
    
    **NOTE:** The Org Unit name must be unique. If the user attempts to
    save an Org Unit with a name that belongs to an existing Org Unit,
    an error message displays. The user must delete this Org Unit and
    re-enter it.

4.  Select a value from the **LIST DATA SOURCE ID** list box.
    
    **NOTE:** This data source contains the table or view that provides
    Org Unit values and must be registered in the platform. Refer to
    [Register a Data Source in
    Common](../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common.htm)
    for more information.

5.  Select a value from the **LIST SOURCE** list box.
    
    **NOTE:** The list source is a table or a list that contains all the
    possible values <span style="text-indent: -20px;">for Org Units.
    There can only be one row per value in the **VALUE FIELD**. For
    example, </span><span style="text-indent: -20px;">the list source
    cannot require a Where clause or be language dependent.</span>

6.  Select a value from the **VALUE FIELD** list box.
    
    **NOTE:** The value field is a column from the list source that
    provides the actual Org Unit values used to process a request, e.g.
    WERKS is the value field that provides Org Unit values for Plant in
    request processing.

7.  Select a value from the **DESCRIPTION FIELD** list box.
    
    **NOTE:** This value is the name of the field that contains the
    description for the <span style="font-weight: bold;">VALUE
    FIELD</span>.
    
    **NOTE:** Description field is optional, but should be chosen if it
    exists in the List Source.

8.  Enter optional text in the **COMMENT** field.

9.  Click <span style="font-weight: bold;">Save.</span>

Continue with Add an Org Unit Type to a Category
Object.

## <span id="Add_an_Org_Unit_Type_to_a_Category_Object"></span>Add an Org Unit Type to a Category Object

A Designer performs this task.

The user identifies whether each category object uses org units and what
those org unit types are. This gives the Content WebApp the ability to
drive data-level security of values within the org units so that users
only see the data that is relevant to their org unit security setup.

Each category object is limited to three org unit types. An org unit
type consists of org units that have been created on the [Org
Units](../Page_Desc/Org_Units.htm) page.

For example, the category Customer uses a category object of Customer
Data. The Customer Data category object uses the Company Code org unit
for org unit type 1 and the SalesOrg org unit for org unit type 2. Org
unit type 3 is not populated.

To add an org unit type to a category in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct </span>**\>
    Design** in the *Navigation* pane; the *Category* page displays.

2.  Click <span style="font-weight: bold;">Vertical View</span> for a
    category **NAME**.

3.  Click the **Org Unit Types** button.

4.  If no records exist, the page displays in add mode. Otherwise, click
    **Add**.
    
    [View the field descriptions for the Category Org Unit Type
    page](../Page_Desc/Category_Org_Unit_Type.htm)

5.  Select a category object from the **OBJECT NAME** list box.
    
    **NOTE**: If no category objects exist for this category, the OBJECT
    NAME defaults to the category name. Refer to the
    [Category](../Page_Desc/Category_H.htm) page for more information.

6.  If a category object must be added, click **Click to add a new
    item**. The *Category Objects* page displays in add mode in another
    browser tab.

7.  Enter the category object name in the **OBJECT NAME** field.

8.  Click **Save**.

9.  Return to the *[Category Org Unit
    Type](../Page_Desc/Category_Org_Unit_Type.htm)* page.

10. Select the newly added category object from the **OBJECT NAME** list
    box.

11. Select an org unit from the **ORGUNIT1TYPE, ORGUNIT2TYPE** or
    **ORGUNIT3TYPE** list boxes as needed.

12. Click
**Save**.

## <span id="Add_and_Configure_Org_Unit_Groups,_Types,_and_Values"></span>Add and Configure Org Unit Groups, Types, and Values

A Security Administrator can add an org unit group and configure the org
unit values for each type of org unit in the org unit group. By
configuring org unit groups a Security Administrator can define a set of
org unit values that can be used in multiple security positions and
roles.

Before performing this task, org units must be added. The org unit types
that can be configured for a group are based on the org unit set up on
the <span style="font-style: italic;">[Org
Units](../Page_Desc/Org_Units.htm)</span> page. Refer to [Add Org
Units](Manage_Org_Units.htm#Add_Org_Units) for more information.

Once an org unit group is added and the values for each org unit type
are configured, the org unit group can be added to positions and roles
in Security. Refer to [Add Org Units from a Group to all Roles in a
Position](Add_Org_Units_from_a_Group_to_Roles.htm#Add_Org_Units_from_a_Group_to_all_Roles_in_a_Position)
and [Add Org Units from a Group to a Position
Role](Add_Org_Units_from_a_Group_to_Roles.htm#Add_Org_Units_from_a_Group_to_a_Position_Role)
for more information.

To add org unit groups and configure org unit values for org unit groups
in dspConduct™:

1.  Select <span style="font-weight: bold;">dspConduct \>
    </span>**Configuration \> Org Units Groups** in the *Navigation*
    pane; the *Org Units Groups* page displays.

2.  If no records exist, the page displays in add mode. Otherwise, click
    **Add**.
    
    *[View the field descriptions for the Org Units Groups
    page.](../Page_Desc/Org_Unit_Groups.htm)*

3.  Enter a unique name in the **NAME** field.

4.  Click **Save**.

5.  Click the **Org Units** icon for the Org Unit Group; the *Org Unit
    Group Types* page displays.
    
    *[View the field descriptions for the Org Units Group Types
    page.](../Page_Desc/Org_Unit_Group_Types.htm)*
    
    **NOTE:** The org unit IDs that display are based on the types of
    org units added on the *[Org Units](../Page_Desc/Org_Units.htm)*
    page.

6.  Click the **Org Units** icon for an Org Unit ID; *Org Unit Group
    Type Values* page displays.
    
    *[View the field descriptions for the Org Units Group Type Values
    page.](../Page_Desc/Org_Unit_Group_Type_Values.htm)*

7.  Select one or more org unit values, and then click the
    <span style="font-weight: bold;">Include</span> or
    <span style="font-weight: bold;">Remove</span> icon as needed.

8.  Repeat Steps 6 and 7 as needed to select org unit values for
    additional org units for the group.
