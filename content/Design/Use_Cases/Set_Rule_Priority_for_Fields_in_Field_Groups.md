+++
title = 'Set Rule Priority for Fields in Field Groups'
solution = 'Migration'
+++

# Set Rule Priority for Fields in Field Groups

A field’s priority determines the order in which the rule based on that
field is run and is set on the *Target Fields* page. In this example,
the PSTAT field’s priority is 4.

All fields are associated with the default field group (\*).

The priority for fields in the default field group  (\*) is set by the
order the field appears in the Target table. If the default field group
(\*) were the only field group used for the PSTAT field for the ttMARA
Target, then no other priority is necessary.

Fields can also be associated with different field groups to apply
different filters to values in the field. In this case, the rule
priority offset helps to define the order in which the filters are
applied and the rules are run on these filtered values.

When using field groups, the order that rules run is important.

The rules assigned to field groups other than default field group (\*)
must run on a subset of data prior to the rules assigned to the default
field group (\*), which run on all data.

When a rule runs, it searches for matches based on those fields that
contain NULL.

If the default field group (\*) rules run first, all NULL values in
fields are replaced with values according to the default field group
(\*) rules. If the rules associated with other field groups run after
the default field group (\*) rules, the rules will not return matches,
because the fields will have been populated according to the default
field group (\*) rules (as in, no fields will contain NULL).Therefore,
rules associated with field groups other than the default field group
(\*) will <span style="color: #ff0000;font-weight: bold;">not</span> be
applied correctly if the rules associated with the default field group
(\*) run first.

For example, the field group FERT runs rules on records with a Material
Type of Finished Goods, setting a default value of 5 in the Maintenance
Status field (PSTAT) for all Finished Goods. This rule has a priority of
36. After this rule runs, the PSTAT field contains 5 for Finished Goods,
and NULL for all other records. The next rule for the default field
group (\*) has a priority of 40, and runs on all records where the PSTAT
value is NULL. If the rules associated with the default field group (\*)
ran first, no values in the PSTAT would be NULL, and the rule associated
with the FERT field group, which searches for NULL values, would not be
applied. This is why setting the priority on the field group for rule
generation is important.

The order that a rule runs depends on the rule’s priority and two other
settings: the Source Priority Multiplier and the Rule Priority Offset.

The **Source Priority Multiplier**, set on the Map tab of the
*[Parameters](../../Console/Page_Desc/Parameters)* page in Console,
is applied to the rule’s priority. If the PSTAT Target field’s priority
is 4 and the Source Priority Multiplier is 10, the rule associated with
that field will be assigned a priority of 40. The priority for the PSTAT
field in the default field group (\*)  is 40, so an additional setting
must be used for other field groups to set them to run prior to the
default field group (\*) .

The **Rule Priority Offset**, which is always a negative number, is set
on the *[Field Groups](../Page_Desc/Field_Groups)* page. This value
is subtracted from the rule’s priority to set the order the rule is run.
If the Rule Priority Offset for the PSTAT field’s field group HALB is
-4, the final priority set for the rule to run in Transform is 36.
 Since the default field group (\*) does not have a Rule Priority
Offset configured (and its priority is 40), it will run after the HALB
field group.
