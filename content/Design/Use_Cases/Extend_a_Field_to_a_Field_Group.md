+++
title = 'Extend a Field to a Field Group'
solution = 'Migration'
+++

# Extend a Field to a Field Group

Field groups are filters used to create subsets of data in a Target
field. Rules, requirement settings, criticality levels and other
settings can then be applied to these subsets of data.

A field can be extended to all field groups assigned to the Object from
the *[Target Fields](../Page_Desc/Target_Fields_H_Target_Design)*
page, allowing this field to have a filter applied based for every field
group.

<span style="font-weight: bold;">NOTE</span>: Fields cannot be extended
to field groups is the Target's Design Status is Design Finished,
Complete or Inactive.

<span style="font-weight: bold;">NOTE</span>: zLegacy fields cannot be
extended to field groups.

To extend a field to a field group in Target Design:

1.  Click **Design** in the Context bar.

2.  Click the **Targets**icon on the *[Design](../Page_Desc/Design)*
    page.

3.  Click the **Target Fields**icon for a Target.
    
    **NOTE**: All Target fields belong to the \* field group by default.

4.  Select the field to extend to all field groups for the Object that
    contains the Target.

5.  Click the **Extend to Field Groups** icon in the Page toolbar; a
    confirmation message display.

6.  Click **OK**.

One record displays on the *Target Fields* page for the field for each
field group in the Object.

For example, if three field groups (FERT, HALB and ROH) have been added
to the Object, and the field MTART has been extended to field groups for
the Object, four records display for the MTART field on the *Target
Fields* page, one for each field group to which the field belongs
(including the \* field group). When the field is brought into Map when
the Target is synced, the four records display for the field on the
*[Field Mappings](../../Map/Page_Desc/Field_Mappings_H)* page, one
for each of the field groups, and mapping can be performed on each
field-field group combination..

To further understand the concept, when a field is extended to field
groups, it is actually added to the default (\*) field group only.
However, all other field groups inherit fields and most other settings
from the default field group(\*). These inherited settings cannot be
changed for field groups.

Some settings are not inherited from the default field group (\*). The
following fields can be updated for each field group when a field is
extended to it:

  - Required
  - Criticality
  - Rules
  - Comments
  - Instructions
  - Documentation
