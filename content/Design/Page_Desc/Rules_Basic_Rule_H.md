+++
title = 'Rules: Basic Rule H'
solution = 'Migration'
+++

# Rules: Basic Rule H

[Rules: Basic Rule V](#Rules)

<div class="use">

Use this page to [Add a Basic Rule](../Use_Cases/Basic_Rules.htm).

</div>

<span style="font-weight: bold;">NOTE:</span> Bulk Execution has been
enabled on this page. Refer to [Use Bulk
Execution](../../../Platform/Bulk_Exec/Use_Bulk_Execution.htm) for more
information.

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Select <span style="font-weight: bold;">Design </span>in the Context
    bar.
3.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Design](Design.htm)* page.
4.  Click the <span style="font-weight: bold;">Basic Rules</span> icon
    for a Target.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>FIELD ORDER</p></td>
<td><p>Displays the order of the field entered on the <span style="font-style: italic;"><a href="Target_Fields_H_Target_Design.htm">Target Fields</a></span> page.</p>
<p>The order is used to sort the <span style="font-style: italic;"><a href="../../Map/Page_Desc/Field_Mappings_H.htm">Field Mappings</a></span> page in Map. Key and required fields are given a lower number (as in, a higher priority) than optional fields.</p>
<p>This value is entered on the <span style="font-style: italic;">Target Fields</span> page’s <span style="font-style: italic;">Vertical</span> View in the Field Order field on the General tab.</p></td>
</tr>
<tr class="odd">
<td><p>TARGET FIELD ID</p></td>
<td><p>Displays the name of the selected active field in the selected Target to which the Basic rule will be applied.</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the Basic rule will be added to the enrichment data flow during Data Services AutoGen if multiple rules are added for the field. This number must be unique.</p></td>
</tr>
<tr class="odd">
<td><p>NAME</p></td>
<td><p>Displays the Basic rule name.</p>
<p>A Basic rule allows a user to create a simple conditional or default rule (one that populates the field with a default value) used in Data Services AutoGen.</p>
<p>For an overview of Basic rules, refer to <a href="../Use_Cases/Basic_Rules.htm#Add">Add a Basic Rule</a>.</p></td>
</tr>
<tr class="even">
<td><p>RULE DESCRIPTION</p></td>
<td><p>Displays a description of the rule that is created based on the properties and conditions. This field is populated by the system from the description that is added on the <span style="font-style: italic;">Vertical</span> View and is for documentation purposes only.</p></td>
</tr>
</tbody>
</table>

## <span id="Rules"></span>Rules Basic Rule V

<div class="use">

Use this page to [Add a Basic Rule](../Use_Cases/Basic_Rules.htm).

</div>

Field

Description

Target Field ID

Displays the name of an active field in the selected Target to which the
Basic rule will be applied.

Priority

Displays the order that the basic rule will be added to the enrichment
data flow during Data Services AutoGen if multiple rules are added for
the field. This number must be unique.

Name

Displays the Basic rule name.

A Basic Rule allows a user to create a simple conditional or default
rule (one that populates the field with a default value).

For an overview of Basic rules, refer to [Add a Basic
Rule](../Use_Cases/Basic_Rules.htm).

Rule Properties

Field Value

Displays the value that will be set for the selected Target field if the
rule condition(s) is met during Data Services AutoGen.

Is Null Condition

If checked and  the value in the Target field is NULL, the field will be
populated with the value in the Field Value field during Data Services
AutoGen. The Is Null Condition works in conjunction with any other rule
condition added for the Target field.

Rule Conditions

RuleField1

Displays the name of the field in the Target that will be evaluated if
the value in the field meets the condition. The Field Value is used for
the selected Target field. Each field can only be used in one condition
per rule.

**NOTE**: If other RuleFields have been added, this condition is
combined with them using an AND operator.

RuleField1Value

Displays the value that, if contained in the RuleField1 field, will meet
the rule’s condition. The Field Value will be set for the Target Field
for the record.

RuleField2

Displays the name of the field in the Target that will be evaluated. If
the value in the field meets the condition, the Field Value is used for
the selected Target field. Each field can only be used in one condition
per rule.

**NOTE**: If other RuleFields have been added, this condition is
combined with them using an AND operator.

RuleField2Value

Displays the value that, if contained in the RuleField2 field, will meet
the rule’s condition. The Field Value will be set for the Target Field
for the record.

RuleField3

Displays the name of the field in the Target that will be evaluated. If
the value in the field meets the condition, the Field Value is used for
the selected Target field. Each field can only be used in one condition
per rule.

**NOTE**: If other RuleFields have been added, this condition is
combined with them using an AND operator.

RuleField3Value

Displays the value that, if contained in the RuleField3 field, will meet
the rule’s condition. The Field Value will be set for the Target Field
for the record.

General

Description

Displays a user-entered description of the rule.
