+++
title = 'Basic Rules'
solution = 'Migration'
+++

# Basic Rules

A Basic rule allows a user to create a simple conditional or default
rule (one that populates the field with a default value).

Basic rules are logic conditions associated with a Target field that are
used in Data Services AutoGen. They can be used to apply conditions
based on up to three combined fields. When Data Services AutoGen runs,
the Basic rules are added to the job in the enrichment data flow based
on the priority set in Target Design. Basic rules are overwritten using
the rule definition from Target Design each time Data Services Jobs are
automatically generated.

Refer to [Data Services
AutoGen](../../Data_Services_AutoGen/Data_Services_Automation.htm) for
more information.

When setting up a Basic rule, the user enters a field value to which the
Target field is set if rule conditions are met. Up to three combined
conditions with an operator of = can be evaluated for each Basic rule.

A Basic rule can be added to a field on the
[*Targets*](../Page_Desc/Targets_H_Design.htm) page or the *[Target
Fields](../Page_Desc/Target_Fields_H_Target_Design.htm)* page. On the
<span style="font-style: italic;">Targets</span> page, a user can select
the field to which the Basic rule is applied. On the
<span style="font-style: italic;">Target Fields</span> page, the user
can assign a Basic rule to a specific field.

<span style="font-weight: bold;">NOTE:</span> Basic rules cannot be
added to zLegacy fields.

**NOTE:** A Basic rule can only be added to a Target field if the Target
has a Design Status of In Design.

Basic rules are managed in Target Design. They are not edited or
submitted in Map. These mappings have a message on the record on the
<span style="font-style: italic;">[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H.htm)</span> page in Map
stating that the rule was created in Target Design. The mapping for a
field with a Basic rule displays in Map with an Action of Rule. If a
field has both a Complex and Basic rule, the mapping displays in Map
with an Action of Manual Rule.

After a Target with a Target field that has a Basic rule assigned is
synced with Map, these rules are automatically sent to the
<span style="font-style: italic;">[Mapping
Approval](../../Map/Page_Desc/Mapping_Approval_H.htm)</span> page for a
developer to review them, however they do not require approval to be
used by Data Services AutoGen.

If a Target’s Source mappings and Target mappings ({Target Rules}) are
complete, and a Basic rule is added to a Target or field, Source
mappings are not overwritten when the Target is synced to Map. Target
mappings (as in, {Target Rules}) are overwritten when the Target is
synced.

This section contains the following topics:

  - [Add a Basic Rule to a Target](#Add)
  - [Add a Basic Rule to a Target Field](#Add2)
  - [Sync Basic Rules with Map](#Sync)

## <span id="Add"></span>Add a Basic Rule to a Target

When a Basic rule is added at the Target level, the user selects the
field to which the rule is applied.

<span style="font-weight: bold;">NOTE:</span> Use single quotes (‘)
around strings when entering values.

To assign a Basic rule to a field at the Target level:

1.  Select **Design** in the Context bar.

2.  Click the **Targets** icon.

3.  Click the **Basic Rules** icon for a Target.
    
    **NOTE:** If no records exist, the page displays in add mode.
    Otherwise, click Add.
    
    *[View the field descriptions for the Rules: Basic Rule
    page](../Page_Desc/Rules_Basic_Rule_H.htm)*

4.  Select the field to which the rule applies in the **TARGET FIELD
    ID** list box.
    
    **NOTE:** Only active fields assigned to the selected Target
    display.
    
    **NOTE:** zLegacy fields do not display and fields that are in field
    groups other than the default field group (\*);do not display.

5.  Enter a value in the **PRIORITY** field.
    
    <span style="font-weight: bold;">NOTE:</span> This is the order that
    the Basic rule will be added to the enrichment data flow during Data
    Services AutoGen if multiple rules are added for the field. This
    number must be unique for a rule / field combination (as in, a rule
    for another Target field can have the same priority number but
    cannot use the same Target field).

6.  Enter a descriptive rule name in the
    <span style="font-weight: bold;">NAME</span>field.

7.  Click **Save**; the *Vertical* View displays.

8.  Enter a value in the **Field Value** field.
    
    **NOTE:** This is the value that the field will be set to if the
    rule condition(s) is met.
    
    **NOTE:** Use single quotes (‘) around strings.

9.  Check the <span style="font-weight: bold;">Is Null Condition</span>
    check box if needed.
    
    <span style="font-weight: bold;">NOTE:</span> If checked, if the
    value in the Target field is NULL, the field will be populated with
    the value in the Field Value field. The Is Null Condition works in
    conjunction with any other rule condition added for the Target
    field.

10. Select a field name in the **Rule Field1** list box.
    
    <span style="font-weight: bold;">NOTE:</span> The values stored in
    this field in the Target are evaluated using the value entered in
    the Rule Field1Value. Each field can only be used in one condition
    per rule.

11. Enter the value that will cause Field Value to be set for the field
    in the **RuleField1Value** field.
    
    <span style="font-weight: bold;">NOTE:</span> Up to three conditions
    can be added. They will be AND combined.
    
    <span style="font-weight: bold;">NOTE:</span> Use single quotes (‘)
    around strings.

12. Click **Save**.

For example, a user sets a Basic rule for the PSTAT field (Maintenance
Status) on the ttMARA table by completing the fields on the
<span style="font-style: italic;">[Rules: Basic
Rule](../Page_Desc/Rules_Basic_Rule_H.htm)</span>page's
<span style="font-style: italic;">Vertical</span> View with these
values.

|                   |       |
| ----------------- | ----- |
| Field             | Value |
| Field Value       | 1     |
| Rule Field1       | MTART |
| Rule Field1 Value | FERT  |

This rule states that if the MTART field (Material Type) on the ttMARA
table has a value of FERT (Finished Goods), the rule condition is met,
and the PSTAT field for that record will be set to 1.

## <span id="Add2"></span>Add a Basic Rule to a Target Field

When a Basic rule is added at the target-field level, the user selects
the rule to apply to the selected field.

<span style="font-weight: bold;">NOTE:</span> Use single quotes (‘)
around strings when entering values.

To add a Basic rule to a target field in Target Design:

1.  Select **Design** in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the **Targets** icon on the
    *[Design](../Page_Desc/Design.htm)* page.

3.  Select the **Fields** icon for a Target.

4.  Click the **Basic Rules** icon for a field.

5.  If no records exist, the page displays in add mode. Otherwise, click
    **Add**.
    
    *[View the field descriptions for the Rules: Basic
    Rule page](../Page_Desc/Rules_Basic_Rule_H.htm)*

6.  Enter a value in the **PRIORITY** field.
    
    **NOTE:** This is the order that the Basic rule will be added to the
    enrichment data flow when the rule is autogenerated during Data
    Services AutoGen if multiple rules are added for the field. This
    number must be unique.

7.  Enter a descriptive rule name in the
    <span style="font-weight: bold;">NAME</span> field.

8.  Click **Save**; the *Vertical* View displays.

9.  Enter a value in the **Field Value** field.
    
    **NOTE:** This is the value that the field will be set to if the
    rule condition(s) is met.
    
    **NOTE:** Use single quotes (‘) around strings.

10. <span>Enable the </span><span style="font-weight: bold;">Is Null
    Condition</span><span> check box if needed</span>.
    
    **NOTE:** If enabled, if the value in the target field is NULL, the
    field will be populated with the value in the Field Value field. The
    Is Null Condition works in conjunction with any other rule condition
    added for the target field.

11. Select a field name in the <span style="font-weight: bold;">Rule
    Field1</span> list box.
    
    **NOTE:** The values stored in this field in the target are
    evaluated using the value entered in the Rule Field1Value field.
    Each field can only be used in one condition per rule.

12. Enter the value that will cause the Field Value field to be set for
    the field in the
    <span style="font-weight: bold;">RuleField1Value</span> field.
    
    **NOTE:** Up to three conditions can be added.
    
    **NOTE:** Use single quotes (‘) around strings.

13. Click <span style="font-weight: bold;">Save</span>.

For example, a user sets a Basic rule for the PSTAT field (Maintenance
Status) on the ttMARA table by completing the fields on the
<span style="font-style: italic;">[Rules: Basic
Rule](../Page_Desc/Rules_Basic_Rule_H.htm)</span> page's
<span style="font-style: italic;">Vertical</span> View with these
values.

|                   |       |
| ----------------- | ----- |
| Field             | Value |
| Field Value       | 1     |
| Rule Field1       | MTART |
| Rule Field1 Value | FERT  |

This rule states that if the MTART field (Material Type) on the ttMARA
table has a value of FERT (Finished Goods), the rule condition is met,
and the PSTAT field for that record will be set to 1.

## <span id="Sync"></span>Sync Basic Rules with Map

Once the fields' Target is synced to Map, the Target Rules for the field
display on the <span style="font-style: italic;">[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H.htm)</span> page in Map.
The fields and their settings are:

  - <span style="font-weight: bold;">Action</span>— Rule
  - <span style="font-weight: bold;">Rule Status</span>— Complete
  - <span style="font-weight: bold;">Mapping Status</span>— Complete
  - <span style="font-weight: bold;">Edit</span>,
    <span style="font-weight: bold;">Reset</span>, and
    <span style="font-weight: bold;">Submit</span> icons are disabled
  - <span style="font-weight: bold;">Rules Comment</span>— Indicates
    that the rule has been added in Target Design
  - <span style="font-weight: bold;">Comment</span>— Indicates that the
    rule has been added in Target Design
  - <span style="font-weight: bold;">Mapped On</span>— Displays the date
    that the target was synced
  - <span style="font-weight: bold;">Mapped By</span>— Displays Target
    Design..

Refer to [Sync Map and Target Design](Sync_Map_and_Target_Design_TD.htm)
for more information.
