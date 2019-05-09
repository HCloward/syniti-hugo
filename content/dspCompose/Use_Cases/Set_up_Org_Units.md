+++
title = 'Set up Org Units'
solution = 'Data Quality'
+++

# Set up Org Units

An Org Unit is tied to a data source, which may be either a list, or a
table that exists in a database such as dgSAP, or a table that has been
created specifically to store Org Units. This data source must exist
prior to setting up Org Units.

The data source stores a column that corresponds to an Org Unit (for
example, a plant, or a division, or a sales organization). This column
provides the Org Unit values (such as specific plants, divisions or
sales organizations).

![](../../../Resources/Images/image005.png)

*Example of a ttCompany table created to be used with an Org Unit*

To set up Org Units:

  - [Create Org Units](#Create_Org_Units)

  - [Assign Users to Org Units](#Assign_Users_to_Org_Units)

  - [Add Org Units to a Template](#Add_Org_Units_to_a_Template)

## <span id="Create_Org_Units"></span>Create Org Units

All Org Units are global and defined at the configuration level.

Once added, an Org Unit cannot be edited. If changes need to be made to
an Org Unit, delete the record and add a new Org Unit.

To create an Org Unit:

1.  Select **Configuration \> Org Units** in the *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Add**.
    
    *[View the field descriptions for the Org Units
    page.](../Page_Desc/Org_Units)*

3.  Enter a name in **ORG UNIT
    <span style="font-weight: normal;">field.</span>**
    
    **NOTE**: This name describes the Org Unit, such as plant or
    division. It can contain all letters, 0-9 and underscores only.
    
    **NOTE**: The Org Unit name must be unique. If the user attempts to
    save an Org Unit with a name that belongs to an existing Org Unit,
    an error message displays. The user must delete this Org Unit and
    re-enter it.

4.  Select an option from the **LIST DATA SOURCE ID** list box.
    
    **NOTE**: This data source contains the table or view that stores
    the Org Unit values and must be registered in the Platform.

5.  Select an option from the **LIST SOURCE** list box.
    
    **NOTE**: The list source is a table or a list that contains all the
    possible values for Org Units. There can only be one row per value
    in the **VALUE FIELD.** For example, the list source cannot require
    a Where clause or be language dependent.

6.  Select an option from the **VALUE FIELD** list box.
    
    **NOTE**: The value field is a column from the list source. This
    list could be a list of plants, divisions or other related working
    groups and will be used in a request to allow users access to
    request data.

7.  Select an option from the **DESCRIPTION FIELD** list box.
    
    **NOTE**: This value is the field that contains the description for
    the **VALUE FIELD**. Description field is optional, but should be
    chosen if it exists in the List Source.

8.  Enter text in **COMMENT**.

9.  Click **Save**.

## <span id="Assign_Users_to_Org_Units"></span>Assign Users to Org Units

Users must be assigned to Org Units and specific Org Unit values.

To assign users to Org Units:

1.  Select **Configuration \> Users** in the *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Org Units** for a user.

3.  Click **Add**.
    
    *[View the field descriptions for the User (Org Units)
    page.](../Page_Desc/User_Org_Units)*

4.  Select an option from the **ORG UNIT ID** list box.

5.  Click **Save**.

6.  Click **Assignments** for an Org Unit.

7.  Click the **ASSIGNED** check box to assign that Org Unit value to
    the selected user.

**NOTE**: Click the **Select All** or **Deselect All** buttons in the
Page toolbar to assign or unassign a user to all Org Unit values.

[View the field descriptions for the User (Org Unit Assignments)
page](../Page_Desc/User_Org_Unit_Assignments)

Org Unit assignments from a template are copied to a request based on
that template, but can be modified at the request level on the *Request
(Org Unit Assignments)* page. Refer to [Configure and Confirm Request
Org Unit Assignments](Request_Org_Unit_Assignments) for more
information.

A user can also reset modified Org Unit assignments at the request level
back to the template level Org Unit assignments. Refer to [Reset the Org
Unit Assignments for a
Request](Request_Org_Unit_Assignments#Reset_the_Org_Unit_Assignments_for_a_Request)
for more information.

**NOTE**: An Org Unit value may become invalid if it is removed from the
list source. If a value in **ORG UNIT VALUES** is deleted from the Org
Unit’s list source, a check mark displays in **VALUE INVALID**. Click
the **Remove Invalid Values** button on the Page toolbar to remove this
value. Any existing user Org Unit assignments to this value are
deleted.

## <span id="Add_Org_Units_to_a_Template"></span>Add Org Units to a Template

One or many Org Units can be assigned to a template.

To add the Org Unit to a template:

1.  Click **Team** on *Navigation
    <span style="font-style: normal;">pane</span>*.

2.  Click **Templates** for a team.

3.  Click **Org Units** for a template.

4.  Click **Add**.
    
    *[View the field descriptions for the Template (Org Units)
    page.](../Page_Desc/Template_Org_Units_H)*

5.  Select an option from the **ORG UNIT ID** list box.

6.  Enter a column name in **TEMPLATE COLUMN** field.
    
    **NOTE**: The TEMPLATE COLUMN represents the Org Unit in the Org
    Unit table that dspCompose™ creates when the template is generated.
    Refer to [TEMPLATE COLUMN Information](#TEMPLATE_COLUMN_Information)
    for additional information.
    
    **NOTE**: For help when completing the TEMPLATE COLUMN field, click
    the **Template Column Display** button on the *[*Template (Org
    Units)*](../Page_Desc/Template_Org_Units_H)*page on the Page
    toolbar for a list of columns in the template. This button is active
    if the template has been recorded in dspCompose™, or if the
    Integrate template assigned to the dspCompose™ template has columns
    and fields defined in Integrate.

7.  Click **Save**.

<span style="font-weight: bold;">NOTE</span>: Click **Org Unit Display**
to view a list of users who can access the Org Unit and their Org Unit
values.

Continue to configure Org Units for templates. Refer to [Set Org Unit
Assignment Security for a
Request](Org_Unit_Objects_Generated_by_dspCompose) for more
information.

## <span id="TEMPLATE_COLUMN_Information"></span>TEMPLATE COLUMN Information

BackOffice recommends that the text entered in the **TEMPLATE COLUMN**
field on the *[*Template (Org
Units)*](../Page_Desc/Template_Org_Units_H)* page correspond to a
column in the template that stores the Org Unit values.

![](../../../Resources/Images/image009.png)

In the example above, the **TEMPLATE COLUMN** value MARA-SPART
corresponds to a Division value on the template.

When the user generates this template, dspCompose™ creates the standard
set of objects, and also creates Org Unit related objects. Refer to [Org
Unit Objects Generated by
dspCompose](Org_Unit_Objects_Generated_by_dspCompose) for more
information.

When the template is generated, dspCompose™ creates an Org Unit table in
the cMass\_Data database for the template with the name tt\[template
name\]OrgUnit. This table contains a column named after the value
entered in TEMPLATE COLUMN in the example above.

![](../../../Resources/Images/image010.png)

To simplify joins between tables, it is a best practice to enter the
name of the column in the template recording in the TEMPLATE COLUMN name
on the *Template (Org Units)* page. If the Template Administrator
chooses to write views that tie other tables, such as the data entry
tables, to the Org Units table, it is easiest if the column names match.

The Org Unit table also contains the request ID and the Org Units for
the request, which are populated when a request based on the template is
saved.

**NOTE:** If the data entry table does not exist when the template is
generated, the security view will not be automatically generated. This
situation can occur when the template is a custom template with custom
data entry pages.

**NOTE:** If the value entered in the **TEMPLATE COLUMN** column on the
*Template (Org Units)* page does not exactly match a column in the data
entry table, that Org Unit will be excluded from the generated security
view. To add the Org Unit, the security view will have to be manually
modified to include a join from the TemplateColumn name in the Org Unit
table to the appropriate column in the data entry table.

Refer to [Incorporate the Security View into Request
Processing](Incorporate_the_Security_View_into_Request_Processing)
for more information.

**NOTE:** There is no automatic linking of Org Units into request
processing. Once the Org Unit table is created and a request that uses
Org Units is saved, it is up to the Template Administrator, using DSP®
development skills to then customize a solution. Refer to [Incorporate
the Security View into Request
Processing](Incorporate_the_Security_View_into_Request_Processing)
for more information.

The Template Administrator could:

  - Join the Org Unit table into the Data Entry View for the request

  - Join the Org Unit table into list boxes to limit valid list box
    values to only those values associated with the Org Unit

  - Use the table to write validation rules

  - Use the table to write control views to allow users to view but not
    edit request data

  - Use the table to write default procedures or default views

**NOTE**: Refer to [Work with Org Unit Assignments at the Request
Level](Org_Unit_Objects_Generated_by_dspCompose) for more
information.
