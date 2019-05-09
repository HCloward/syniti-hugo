+++
title = 'Automation SQL Field Mappings H'
solution = 'Migration'
+++

# Automation SQL Field Mappings H

[Automation SQL Field Mappings V](#Automation_SQL_Field_Mappings_V)

<div class="use">

Use this page to:

  - [Create Rules](../Use_Cases/Create_Rules)
  - [Reset A Mapping](../Use_Cases/Reset_A_Mapping)

</div>

To access this page:

1.  Click the **Automation** tab on the Quick Panel.
2.  Click the **Mappings** icon for an Object.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Create and Complete</p></td>
<td><p>Click to build a view and a stored procedure for the selected field mapping in the object database. The rule is automatically registered in Transform.</p>
<p><strong>NOTE:</strong> Rules can be created for one mapping at a time.</p>
<p><strong>NOTE:</strong> After the user clicks this icon, the Rule Status is set to Complete.</p>
<p><strong>NOTE:</strong> If the target is in a Design Status of Inactive or Complete, this icon is disabled.</p></td>
</tr>
<tr class="odd">
<td><p>Reset</p></td>
<td><p>Click to clear the Mapping Status and Rule Status for the selected field mapping on the <em><a href="../../Map/Page_Desc/Field_Mappings_H">Field Mappings</a></em> page in Map. This process allows the mapper to remap the field.</p>
<p><strong>NOTE:</strong> When a user clicks Reset, the Created By field on the Vertical View of the Field Mappings page is updated to display the user name of the user who clicked Reset. The Created On field, on the Vertical View of the Field Mappings page, is updated to reflect the date of the reset.</p>
<p><strong>NOTE:</strong> Rules can be reset for one mapping at a time.</p>
<p><strong>NOTE:</strong> The Reset Field Mapping parameter set in Console on the <em><a href="../../Console/Page_Desc/Parameters">Parameters</a></em> page controls how a mapping is updated when it is reset. Options are:</p>
<ul>
<li><p><strong>Reset all Field Mapping Fields</strong> – All fields are cleared of values</p>
<p><strong>NOTE:</strong> If the mapping is associated with a field group other than the default field group (* or “All”), the Target Relationship ID field is not updated on a reset.</p></li>
<li><strong>Reset Status Fields only</strong> – All fields retain values except for the Mapping Status and Rule Status, which are set to Pending Review.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Reject</p></td>
<td><p>Click to reject the selected mapping(s).</p>
<p>If the mapping action is Rule or RuleXref, the Rule SQL field must also have beencompleted with the correct SQL for the rule in the rule comment field.</p>
<p><strong>NOTE:</strong> If the target is in a Design Status of Inactive or Complete, this icon is disabled.</p></td>
</tr>
<tr class="odd">
<td><p>Review Mappings</p></td>
<td><p>Click to open the <em><a href="../../Map/Page_Desc/Field_Mappings_H">Field Mappings</a></em> page in Map for the selected mapping.</p></td>
</tr>
<tr class="even">
<td><p>METRIC GROUP</p></td>
<td><p>Displays the name of the Metric Group added in Target Design Metric groups are a category of field groups that organize and prioritize fields in field groups for mapping.</p></td>
</tr>
<tr class="odd">
<td><p>FIELD GROUP</p></td>
<td><p>Displays the name of the field group to which the field belongs. All fields are assigned to the default field group (*). Field groups are used to organize data to be able to apply different rules, criticality levels, requirements settings against each group depending on the values of data in a related field.</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the order that fields should be mapped, and the order that fields display on the <em><a href="../../Map/Page_Desc/Field_Mappings_H">Field Mappings</a></em> page in Map. Field priority is set on the <span style="font-style: italic;"><a href="../../Design/Page_Desc/Target_Fields_H_Target_Design">Target Fields</a></span> page in Target Design in the Field Order field.</p></td>
</tr>
<tr class="odd">
<td><p>TARGET FIELD</p></td>
<td><p>Displays the name of the target and field selected on the <em><a href="../../Map/Page_Desc/Field_Mappings_H">Field Mappings</a></em>page. The second line will display the description of the field enter in Target Design.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE DETAILS</p></td>
<td><p>Displays the source system name and the Add Row source.</p>
<p>If the Source System says “SELECT SOURCE,” no source has been selected. If it says “{Target Rules},” the rule is a target rule.</p>
<p><strong>NOTE:</strong> If the target field is a key field on the target table, a key icon displays to the right of the field name.</p></td>
</tr>
<tr class="odd">
<td><p><span id="Mapping Actions" class="popUpLink">ACTION</span></p></td>
<td><p>Displays action used to map the field, such as Copy, Default, or Rule.</p>
<p>Values are:</p>
<ul>
<li>Construction</li>
<li>Copy</li>
<li>Default</li>
<li>Internal</li>
<li>Manual Rule</li>
<li>Manual Construction</li>
<li>Not Used</li>
<li>Rule</li>
<li>Rule Xref</li>
<li>Xref</li>
</ul></td>
</tr>
<tr class="even">
<td><p>LOOKUP</p></td>
<td><p>Displays the name of the lookup table created in Target Design. Lookup tables can be viewed for mappings with any action. In AutoGen, lookup tables are used with mappings that have an action of RuleXref and Rule.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE TABLE</p></td>
<td><p>Displays source table used for Copy, RuleXref, Xref or Construction actions.</p>
<p><strong>NOTE:</strong> When mapping a source, this field displays the Add Row and Update Row sources for the Add Row source only. When mapping a target, the field displays any target in the Wave and Process Area.</p></td>
</tr>
<tr class="even">
<td><p>RULES COMMENT</p></td>
<td><p>Displays technical information entered by the Mapper to help the Developer build the rule when the action for the mapping is Manual Rule.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE FIELD</p></td>
<td><p>Displays source field used for Copy, RuleXref, Xref or Construction actions.</p></td>
</tr>
<tr class="even">
<td><p>DEFAULT VALUE</p></td>
<td><p>Displays data used in the default rule creation process (for example, when ACTION is set to Default). For actions other than Default, this field is &lt;Blank&gt;. Enter &lt;Blank&gt; to indicate the field does not have a default value. The value will be automatically set to a space (' ').</p></td>
</tr>
<tr class="odd">
<td><p>RULE SQL</p></td>
<td><p>Displays the SQL for the rule entered on the Mapping Approvals page. A developer must enter SQL when rejecting a mapping that has a Manual, Rule or RuleXref action.</p></td>
</tr>
<tr class="even">
<td><p>CREATED ON</p></td>
<td><p>Displays date and time when a user clicked the Create and Complete icon on this page or the Create and Approve Rules icon on the <a href="Automation_page">Automation</a> page to create the rules for the approved mapping.</p></td>
</tr>
<tr class="odd">
<td><p>CREATED BY</p></td>
<td><p>Displays the user ID of the user who clicked the Create and Complete icon on this page or the Create and Approve icon on the <a href="Automation_page">Automation</a> page.</p></td>
</tr>
<tr class="even">
<td><p>MAPPING STATUS</p></td>
<td><p>Displays an icon that represent the <span id="Mapping Status" class="popUpLink">Mapping Status</span> of the field in the mapping process.</p>
<ul>
<li>A red icon indicates a Mapping Status of Pending Review.</li>
<li>A yellow icon represents Design Required.</li>
<li>A green icon is Complete.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>RULE STATUS</p></td>
<td><p>Displays an icon representing the <span id="Rule Status" class="popUpLink">Rule Status</span> of the rule to be built from the mapping once it is complete.</p>
<ul>
<li>A red icon indicates a Rule Status of Pending Review.</li>
<li>A yellow icon represents Revision Requested or that the associated mapping has been submitted and is waiting for Developer review.</li>
<li>A green icon is Complete.</li>
</ul>
<p>Rule status can be updated. Refer to <a href="../Use_Cases/Update_a_Rule_Status">Update a Rule Status</a> for more information.  </p></td>
</tr>
<tr class="even">
<td><p>Log</p></td>
<td><p>Click to open the AutoGen SQL Log page and view successful or failed AutoGen tasks.</p>
<p><strong>NOTE:</strong> If the icon is disabled, no source tables, target tables or rules have been generated for the selected object.</p></td>
</tr>
</tbody>
</table>

## <span id="Automation_SQL_Field_Mappings_V"></span>Automation SQL Field Mappings V

[Automation SQL Field Mappings H](Automation_SQL_Field_Mappings_H)

### General

Field

Description

Reject

Click to reject the selected mapping(s).

If the mapping action is Rule or RuleXref, the Rule SQL field must also
have beencompleted with the correct SQL for the rule in the RULE COMMENT
field.

**NOTE:** If the target is in a Design Status of Inactive or Complete,
this icon is disabled.

Status

Mapping Status

Displays the <span id="Mapping Status" class="popUpLink">Mapping
Status</span> of the field in the mapping process.

Rule Status

Displays the <span id="Rule Status" class="popUpLink">Rule Status</span>
of the rule to be built from the mapping once it is complete.

Rule status can be updated in SQL AutoGen on this  page. Refer to
[Update a Rule Status](../Use_Cases/Update_a_Rule_Status) for more
information.

Mapping

Source

Displays name of the source used in field mapping.

Lookup

Displays the name of the lookup table created in Target Design. Lookup
tables can be viewed for mappings with any action. In AutoGen, lookup
tables are used with mappings that have an action of RuleXref and Rule.

Target Relationship ID

Displays the name of the table that is joined to the current table in a
relationship.

Relationships join Add Row and Update Row sources. If the field is
blank, then the target for the selected mapping is not joined to another
target.

Instruction

Displays the system-generated summary about the field mapping.

Additional Notes

Displays user-entered notes about the mapping.

Rule Details

Auto Generate Rule

If checked, the rule for the field mapping is generated when the user
clicks the Create and Complete icon on the
<span style="font-style: italic;">Horizontal</span> View.

Rule Name

Displays the rule name of the rule to be autogenerated.

**NOTE:** Rule names must follow naming conventions. Refer to [Naming
Convention](../../Transform/Use_Cases/Naming_Conventions)s for more
information.

### Audit Information

Field

Description

Tracking

Mapped By

Displays user ID of individual who selected Complete in the Mapping
Status list box on the *[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H)* page in Map.

Mapped On

Displays date and time when field mapping completed, for example, when
the MAPPING STATUS field was set to Complete on the Field Mappings page
in Map.

Submitted By

Displays user ID of individual who clicked Submit for the mapping on the
<span style="font-style: italic;">[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H)</span> page. The
mapping can then be approved or rejected on the
<span style="font-style: italic;">[Mapping
Approval](../../Map/Page_Desc/Mapping_Approval_H)</span> page.

Submitted On

Displays date and time when the user clicked Submit for the mapping on
the *Field Mappings* page.

Created By

Displays user ID of individual who clicked the Create and Approve Rules
icon on the
<span style="font-style: italic;">[Automation](Automation_page)</span>
page or the Create and Complete icon on this page  to create the rules
for the approved mapping.

Created On

Displays date and time when a user clicked the Create and Approve Rules
icon on the
<span style="font-style: italic;">[Automation](Automation_page)</span>
page or the Create and Complete icon on this page  to create the rules
for the approved mapping.

Approved By

Displays the user ID of the user who approved the rule on the Create and
Approve Rules icon on the
<span style="font-style: italic;">[Automation](Automation_page)</span>
page

**NOTE:** If the rule has not been approved this field is blank. Rules
do not need to be approved to be autogenerated.

Approved On

Displays date and time when rule was approved on the
<span style="font-style: italic;">[Mapping
Approval](../../Map/Page_Desc/Mapping_Approval_H)</span> page.

**NOTE:** If the rule has not been approved this field is blank. Rules
do not need to be approved to be autogenerated.

Rejected By

Displays the user ID of the user who rejected the rule on the
<span style="font-style: italic;">[Mapping
Approval](../../Map/Page_Desc/Mapping_Approval_H)</span> page or on
this page.

**NOTE:** If the rule has not been rejected this field is blank. Rules
do not need to be reviewed to be autogenerated.

Rejected On

Displays date and time when rule was rejected on the
<span style="font-style: italic;">[Mapping
Approval](../../Map/Page_Desc/Mapping_Approval_H)</span> page or on
this page.

**NOTE:** If the rule has not been rejected this field is blank. Rules
do not need to be reviewed to be autogenerated.
