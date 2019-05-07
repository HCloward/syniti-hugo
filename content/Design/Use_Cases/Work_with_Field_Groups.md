+++
title = 'Work With Field Groups'
solution = 'Migration'
+++

# Work With Field Groups

Field groups are filters used to create subsets of data in a Target
field. Based on values in another related field, these subsets can have
different settings, such as criticality, whether the field is required
or which rules will run against the field. If, for example, a field is
required only under certain data conditions, field groups are used to
define the conditions, fields, values, and requirement setting.

**NOTE**: Refer to [Set Rule Priority for Fields in Field
Groups](Set_Rule_Priority_for_Fields_in_Field_Groups.htm) for important
information about the order in which rules assigned to field groups are
run.

The default field group (\*) applies to all data in the Target field, so
rules assigned to this field group run on all data in the fields.

**NOTE  **: All field groups assigned to a Target do not have to be used
for each field mapping. However, the default field group (\*) is
required for all active fields.

For example, the ttMARA table in SAP stores general material data. The
field MTART on that table stores the material type. Material types
include FERT (Finished Goods), HALB (Semi Finished Goods) and ROH (Raw
Materials).

Field groups can be created based on material types, so that rules can
be run on all Finished Goods, all Semi-Finished Goods, and so on. Naming
each field group after the filter value it is based on is a good
practice.

Refer to <span style="font-family: Arial, sans-serif;">[Create Field
Groups](Create_Field_Groups.htm)</span> for more information.

Material types are assigned a Maintenance Status in the PSTAT field on
the ttMARA table. Examples of Maintenance Status are Work Scheduling,
Accounting, or Purchasing.

If all Material Types in the Target should have the same Maintenance
Status, a mapper can create a mapping for the PSTAT field with a Default
action, supply the Default Value (for example, 1) that should be written
to the PSTAT field for every Material Type and apply the rule to the
default field group (\*).  When the rule runs in Transform, the Target
field PSTAT is set to 1 for all Material Types (FERT, HALB and ROH) in
the Target.

In cases where each Material Type (FERT, HALB, and ROH) should have a
different Maintenance Status set in the Target, the mapper submits a
mapping with a different action for each field group.

For example, the mapper can submit a field mapping for the Finished
Goods field group (FERT). In this mapping, the PSTAT field will be
mapped with a Default action, with a Default Value set to 5. When the
rule runs in Transform, records with a Material Type of Finished Goods
will have a Maintenance Status in the Target set to 5.

The mapper can then create a field mapping for the Semi-Finished Goods
field group (HALB). In this mapping, the PSTAT field will be mapped with
a Default action, with a Default Value set to 3. When the rule runs in
Transform, records with a Material Type of Semi-Finished Goods will have
a Maintenance Status in the Target set to 3.

To work with field groups:

  - [Create Field Groups](Create_Field_Groups.htm)
  - [Assign a Field Group to an
    Object](Assign_a_Field_Group_to_an_Object.htm)
  - [Extend a Field to a Field
    Group](Extend_a_Field_to_a_Field_Group.htm)
  - [Set Rule Priority for Fields in Field
    Groups](Set_Rule_Priority_for_Fields_in_Field_Groups.htm)

A user can also:

  - [Set Rule Priority for Fields in Field
    Groups](Set_Rule_Priority_for_Fields_in_Field_Groups.htm)
  - [Use Field Groups](Use_Field_Groups.htm)
