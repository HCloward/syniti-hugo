+++
title = 'Use Field Groups'
solution = 'Migration'
+++

# Use Field Groups

Field groups are filters used to create subsets of data in a Target
field. Based on values in another related field, these subsets can have
different settings that define whether the field is required or which
rules run against the field. If, for example, a field is required only
under certain data conditions, field groups are used to define the
conditions, fields, values, and requirement setting.

By default, field groups use the default (\*) filter, indicating that
all data in the table is available for mapping.

Subsets of data can be based on a field group in the Source table or the
Target table.

If the filter table is the Source table (for example, Filter Table:
MARA, Source Database Object in Map: Mara), begin by configuring the
field group:

1.  [Create Field Groups](Create_Field_Groups).
2.  [Assign a Field Group to an
    Object](Assign_a_Field_Group_to_an_Object).
3.  [Extend a Field to a Field
    Group](Extend_a_Field_to_a_Field_Group).

Continue by mapping the field group fields (as in, the subset of fields
in the Source table):

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Map</span> in the Context
    bar.
3.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Design](../Page_Desc/Design)* page.
4.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.
5.  Click the <span style="font-weight: bold;">Mappings</span> icon for
    a Source in the child pane.
6.  Map each field for the field group. Refer to [Perform Field
    Mapping](../../Map/Use_Cases/Perform_Field_Mapping) for more
    information.

If the filter table is the Target table (for example, Filter Table:
MARA, Target: ttMara), begin by configuring the field group:

1.  [Create Field Groups](Create_Field_Groups).

2.  [Assign a Field Group to an
    Object](Assign_a_Field_Group_to_an_Object).

3.  [Extend a Field to a Field
    Group](Extend_a_Field_to_a_Field_Group).

4.  Add the filter field to the Target table.
    
    **NOTE:** If the filter field does not exist on the Target table,
    create Manual Rules instead of creating field groups. This method
    saves time as a user does not have to create a relationship for each
    field group field. Refer to [Manual
    Rules](../../Map/Use_Cases/Manual_Rule) for more information.

Continue by mapping the field group fields (as in, the subset of fields
in the Target table):

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Map</span> in the Context
    bar.

3.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *Design* page.

4.  Click the <span style="font-weight: bold;">Field Groups</span> icon
    for a Target.

5.  Click the <span style="font-weight: bold;">Mappings</span> icon for
    the field group in the child pane.

6.  Map the fields with the Source Details of {Target Rules}. Refer to
    [Perform Field
    Mapping](../../Map/Use_Cases/Perform_Field_Mapping) for more
    information.

If the filter table is not the Source table (for example, Filter Table:
MARA, Source Database Object in Map: Marc or Filter Table: MARA, Source
Database Object in Map: F0411), begin by configuring the field group:

1.  [Create Field Groups](Create_Field_Groups).
2.  [Assign a Field Group to an
    Object](Assign_a_Field_Group_to_an_Object).
3.  [Extend a Field to a Field
    Group](Extend_a_Field_to_a_Field_Group).

Continue by mapping the field group fields:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Map</span> in the Context
    bar.

3.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *Design* page.

4.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.

5.  Click the <span style="font-weight: bold;">Mappings</span> icon for
    a Source.

6.  Assign a relationship to each of the mappings with a Where clause on
    the <span style="font-style: italic;">Vertical</span> View of the
    <span style="font-style: italic;">[Relationship
    Joins](../../Map/Page_Desc/Relationship_Joins_H)</span> page to
    establish which filter is applied. Refer to [Add Relationship Joins
    to
    Sources](../../Map/Use_Cases/Add_Relationship_Joins_to_Source)
    for more information.
    
    Or
    
    Enter a Where clause for the mapping on the
    <span style="font-style: italic;">Vertical</span> View of the
    <span style="font-style: italic;">[Field
    Mappings](../../Map/Page_Desc/Field_Mappings_H)</span> page.

<span style="font-weight: bold;">NOTE</span>: Enter the source table
name before the field name in the Where clause.
