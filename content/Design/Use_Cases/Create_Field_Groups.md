+++
title = 'Create Field Groups'
solution = 'Migration'
+++

# Create Field Groups

Field groups are filters used to create subsets of data in a Target
field. Rules, requirement settings, criticality levels and other
settings can then be applied to these subsets of data.

The default field group (\*) is automatically created for all Targets.
This field group designates the default action and specifies that the
rule applies to the entire Target and is not dependent on a subset of
data.

For example, to filter on finished goods for SAP, FILTER TABLE = MARA,
FIELD FIELD = MTART and FILTER VALUE = FERT.

Once a field group has been added, assign it to an object so that it can
be applied to the fields in the Targets in that object. Refer to [Assign
a Field Group to an Object](Assign_a_Field_Group_to_an_Object) for
more information.

<span style="font-weight: bold;">NOTE</span>: The default field group
(\*) cannot be edited or deleted.

To create a field group in Target Design:

1.  Select <span style="font-weight: bold;">Configuration \> Field
    Groups</span> in the Navigation pane.

2.  Click <span style="font-weight: bold;">Add</span>.
    
    *[View the field descriptions for the Field Groups
    page](../Page_Desc/Field_Groups)*

3.  Enter a field group name in the
    <span style="font-weight: bold;">NAME</span> field.
    
    <span style="font-weight: bold;">NOTE</span>: Naming each field
    group after the filter value it is based on is a good practice.

4.  Enter a brief description of the filter value in the
    <span style="font-weight: bold;">DESCRIPTION</span> field.

5.  Enter the table that contains the filter value in the
    <span style="font-weight: bold;">FILTER TABLE</span> field.

6.  Enter the field that contains the filter value in the
    <span style="font-weight: bold;">FILTER FIELD </span>field.

7.  Enter the value to filter on in the
    <span style="font-weight: bold;">FILTER VALUE</span> field.
    
    <span style="font-weight: bold;">NOTE</span>: Enter an offset value
    used to run the filter updates prior to running the default field
    group (\*) rule to an update field in the **RULE PRIORITY OFFSET**
    field. Refer to  <span style="font-family: Arial, sans-serif;">[Set
    Rule Priority for Fields in Field
    Groups](Set_Rule_Priority_for_Fields_in_Field_Groups)</span> for
    more information.

8.  Click <span style="font-weight: bold;">Save</span>.
