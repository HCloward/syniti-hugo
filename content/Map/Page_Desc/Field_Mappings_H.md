+++
title = 'Field Mappings H'
solution = 'Migration'
+++

# Field Mappings H

[Field Mappings V](#Field_Mappings_V)

<div class="use">

Use this page to:

  - [Perform Field Mapping](../Use_Cases/Perform_Field_Mapping.htm)
  - [Work with Target Sources that have Multi-part
    Keys](../Use_Cases/Work_with_Sources_with_Multipart_Keys.htm)
  - [Build a Remediation
    Report](../Use_Cases/Build_a_Remediation_Report.htm)

</div>

<span style="font-weight: bold;">NOTE:</span> Bulk Execution has been
enabled on this page. Refer to [Use Bulk
Execution](../../../Platform/Bulk_Exec/Use_Bulk_Execution.htm) for more
information.

To view all field mappings for the selected Target in Map:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Select <span style="font-weight: bold;">Map </span>in the Context
    bar.
3.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area Launch](Process_Area_Launch_map.htm)* page.
4.  Click the <span style="font-weight: bold;">Mappings</span> icon for
    a Target.

To view all field mappings for the selected Target Source in Map:

1.  Click <span style="font-weight: bold;">Map</span> in the Context
    bar.
2.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *Process Area Launch* page.
3.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.
4.  Click the <span style="font-weight: bold;">Mappings</span> icon for
    a Source.

To view all mappings for fields in a field group in Map:

1.  Click <span style="font-weight: bold;">Map</span> in the Context
    bar.
2.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *Process Area Launch* page.
3.  Click the <span style="font-weight: bold;">Field Groups</span> icon
    for a Target.
4.  Click the <span style="font-weight: bold;">Mappings</span> icon for
    a field group.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Submit</p></td>
<td><p>Click to build a view and a stored procedure for the selected field mapping(s) in the object database. This process creates a record on the <em><a href="Mapping_Approval_H.htm">Mapping Approval</a></em> page for the Developer to review. The rule can then be registered in Transform.</p>
<p>After the mapping has been created, the following fields  do not allow update:</p>
<ul>
<li>Action</li>
<li>Source Table</li>
<li>Source Field</li>
<li>Default Value</li>
<li>RULE SQL</li>
</ul>
<p>The fields can be updated after:</p>
<ul>
<li>The Mapper clicks Reset on the <em>Field Mappings</em> page.</li>
</ul>
<p><strong>NOTE:</strong> When a user clicks Reset, the Submitted By field, on the <em>Vertical</em> View of the <em><a href="#">Field Mappings</a></em> page is updated to display the user name of the user who clicked Reset. The Submitted On field, on the <em>Vertical</em> View of the <em>Field Mappings</em> page, is updated to reflect the date of the reset.</p>
<ul>
<li>The Developer clicks Revision Requested on the <em><a href="Mapping_Approval_H.htm">Mapping Approval</a></em> page</li>
</ul>
<p>Once the fields allow update, the user can edit them, then click Save and click Submit. This updated mapping is sent to the Developer for review on the <span style="font-style: italic;">Mapping Approval</span> page.</p></td>
</tr>
<tr class="odd">
<td><p>Sync From Target Design</p></td>
<td><p>Click to sync Map with Target Design, updating tables, fields, Sources and lookup tables.</p>
<p>When Map and Target Design are out of sync, the message &quot;Pending Design Changes&quot; displays to the right of the page name.</p></td>
</tr>
<tr class="even">
<td><p>Reset</p></td>
<td><p>Click to clear the Mapping Status and Rule Status for the selected field mapping(s). This process allows the mapper to remap the field(s).</p>
<p><strong>NOTE:</strong> When a user clicks Reset, the Submitted By field, on the <em>Vertical</em> View of the <em>Field Mappings</em> page, is updated to display the user name of the user who clicked Reset. The <span>Submitted</span> On field, on the <em>Vertical</em> View of the <em>Field Mappings</em> page, is updated to reflect the date of the reset.</p>
<p><strong>NOTE:</strong> The Reset Field Mapping parameter set in Console on the <em><a href="../../Console/Page_Desc/Parameters.htm">Parameters</a></em> page controls how a mapping is updated when it is reset.</p>
<div>
<p>Options are:</p>
<ul>
<li><strong>Reset all Field Mapping Fields</strong> – All fields are cleared of values</li>
</ul>
<p><strong>NOTE</strong>: If the mapping is associated with a field group other than the default field group (* or “All”), the Target Relationship ID field is not updated on a reset.</p>
<ul>
<li><strong>Reset Status Fields only</strong> – All fields retain values except for the Mapping Status and Rule Status, which are set to Pending Review.</li>
</ul>
</div></td>
</tr>
<tr class="odd">
<td><p>Bulk Action</p></td>
<td><p>Click to submit the selected mappings that are in Completed status that have not yet been submitted.</p>
<p>Fields that have basic rules or complex rules assigned in Target Design are not updated. If a rule is set in Target Design, that rule is owned by Target Design. When the rule is pushed to Map, a note attached to the mapping record indicates that the rule has already been set in Target Design and cannot be updated in Map.</p></td>
</tr>
<tr class="even">
<td><p>Submit All</p></td>
<td><p>Click to submit all mappings with a Mapping Status of In Progress and Complete (if that Mapping Status was set manually by the user but had not yet been submitted).</p></td>
</tr>
<tr class="odd">
<td><p>Field Details</p></td>
<td><p>Click to open the <em><a href="../../Design/Page_Desc/Target_Fields_H_Target_Design.htm">Target Fields</a></em> page in Target Design to view details about the selected field.</p></td>
</tr>
<tr class="even">
<td><p>History</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Field_Mapping_History.htm">Field Mapping History</a></span> page to view the history of the mapping for the selected field.</p></td>
</tr>
<tr class="odd">
<td><p>View all Waves Mappings</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Field_Mappings_by_Target_Field_All_Waves.htm">Field Mappings by Target Field (All Waves)</a></span> page to view a history of all mappings across all Waves and Process Areas (from System Types) for the selected field. A user can also copy a mapping to the selected Target or Source.</p></td>
</tr>
<tr class="even">
<td><p>METRIC GROUP</p></td>
<td><p>Displays the name of the Metric Group added in Target Design Metric groups are a category of field groups that organize and prioritize fields in field groups for mapping.</p></td>
</tr>
<tr class="odd">
<td><p>FIELD GROUP</p></td>
<td><p>Displays the name of the field group filter used to organize fields into subsets so that different rules, criticality levels, requirements settings and documentation can be set for these subsets based on values in related fields.</p></td>
</tr>
<tr class="even">
<td><p>FIELD PRIORITY</p></td>
<td><p>Displays the order that fields should be mapped, and the order that fields display on the <span style="font-style: italic;">Field Mappings</span> page in Map. Field priority is set on the <span style="font-style: italic;"><a href="../../Design/Page_Desc/Target_Fields_H_Target_Design.htm">Target Fields</a></span> page in Target Design in the Field Order field.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE DETAILS</p></td>
<td><p>Displays the Source system name and the Add Row Source. From left to right, the fields are: Source System + Source Table (to the left of the arrow), Target (to the right of the arrow), Target Field Name (in red text), Field groups (“All” means that the default field group * is applied), Description of Target Field.</p>
<p>If the Source System says “SELECT SOURCE,” no Source has been selected. If it says “{Target Rules},” the rule is a Target rule.</p>
<p><strong>NOTE:</strong> If the Target field is a key field on the Target table, a key icon displays to the right of the field name.</p>
<p><strong>NOTE:</strong> If an External Source is used in the mapping, the external Source name displays.</p></td>
</tr>
<tr class="even">
<td><p><span id="Mapping Actions" class="popUpLink">ACTION</span></p></td>
<td><p>Displays action used to map field. Refer to <a href="../Use_Cases/Perform_Field_Mapping.htm#Select_an_Action">Select an Action</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>LOOKUP</p></td>
<td><p>Displays the name of the lookup table created in Target Design. Lookup tables can be viewed for mappings with any action. In AutoGen, lookup tables are used with mappings that have an action of RuleXref and Rule.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE TABLE</p></td>
<td><p>Displays Source table used for Copy, RuleXref, Xref or Construction actions.</p>
<p><strong>NOTE:</strong> When mapping a Source, this field displays the Add Row and Update Row Sources for the Add Row Source only. When mapping a Target, the field displays any Target in the Wave and Process Area.</p></td>
</tr>
<tr class="odd">
<td><p>RULES COMMENT</p></td>
<td><p>Displays technical information entered by the Mapper to help the Developer build the rule when the action for the mapping is Manual Rule.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE FIELD</p></td>
<td><p>Displays Source field used for Copy, RuleXref, Xref or Construction actions.</p></td>
</tr>
<tr class="odd">
<td><p>DEFAULT</p></td>
<td><p>Displays data used in the default rule creation process (as in, when ACTION is set to Default). For ACTIONS other than Default, this field is &lt;Blank&gt;.</p>
<p>While mapping a field with the Default action, a user can create output values for blank, empty, and null values. The rule created by the mapping uses these output values. If the user enters &lt;blank&gt; in this field, the output used in the rule is single quotes with one space between them (' '). If the user enters &lt;empty&gt;, the rule uses single quotes with no space between them (''). If the user enters &lt;null&gt;, the rules uses NULL, representing no data.</p></td>
</tr>
<tr class="even">
<td><p>RULE SQL</p></td>
<td><p>Displays the SQL for the rule entered on the <span style="font-style: italic;"><a href="Mapping_Approval_H.htm">Mapping Approval</a></span> page. A developer must enter SQL when rejecting a mapping that has a Manual, Rule or RuleXref action.</p></td>
</tr>
<tr class="odd">
<td><p>MAPPING STATUS</p></td>
<td><p>Displays an icon that represents  the <span id="Mapping Status" class="popUpLink">Mapping Status</span> of the field in the mapping process.</p>
<ul>
<li>A red icon indicates a Mapping Status of Pending Review.</li>
<li>A yellow icon represents Design Required.</li>
<li>A green icon is Complete.</li>
</ul>
<p>A user can update the Mapping Status on the <span style="font-style: italic;">Vertical</span> View.</p></td>
</tr>
<tr class="even">
<td><p>RULE STATUS</p></td>
<td><p>Displays an icon representing the <span id="Rule Status" class="popUpLink">Rule Status</span> of the rule to be built from the mapping once it is complete.</p>
<ul>
<li>A red icon indicates a Rule Status of Pending Review.</li>
<li>A yellow icon represents Revision Requested or that the associated mapping has been submitted and is waiting for Developer review.</li>
<li>A green icon is Complete.</li>
</ul>
<p>Rule status is updated by the system and cannot be changed by the user in Map.</p>
<p>Rule status can be updated in SQL AutoGen on the <a href="../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H.htm">Automation SQL Field Mappings</a> page. Refer to <a href="../../SQL_AutoGen/Use_Cases/Update_a_Rule_Status.htm">Update a Rule Status</a> for more information.  </p></td>
</tr>
</tbody>
</table>

## <span id="Field_Mappings_V"></span>Field Mappings V

[Field Mappings H](Field_Mappings_H.htm)

<div class="use">

Use this page to:

  - [Perform Field Mapping](../Use_Cases/Perform_Field_Mapping.htm)
  - When adding a [Rule](../Use_Cases/Rule.htm) action to a mapping
  - [Build a Remediation
    Report](../Use_Cases/Build_a_Remediation_Report.htm)

</div>

This page has the following tabs:

  - [General](#General_tab)
  - [Audit Information](#Audit_Information_tab)

## <span id="General_tab"></span>General tab

Field

Description

Status

Mapping Status

Displays  the <span id="Mapping Status" class="popUpLink">Mapping
Status</span> of the field in the mapping process.

Rule Status

Displays the <span id="Rule Status" class="popUpLink">Rule Status</span>
of the rule to be built from the mapping once it is complete.

Rule status is updated by the system and cannot be changed by the user
in Map.

Rule status can be updated in SQL AutoGen on the [Automation SQL Field
Mappings](../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H.htm)
page. Refer to [Update a Rule
Status](../../SQL_AutoGen/Use_Cases/Update_a_Rule_Status.htm)for more
information.  

Mapping

Source

Displays name of the Source used in field mapping.

External Source ID

Displays the name of the External Source if one is used in the mapping.
If the field is blank, an external Source was not used.

An External Source is an Update Row Source that is external to the
system used in the Add Row Source when establishing a relationship.

Sources are designated as External Sources in Target Design.

**NOTE:** This list box displays Update Row Sources only. An Add Row
Source cannot be used as an External Source type. The External Source
table must be registered as an Update Row first.

Refer to [Add an External
Source](../Use_Cases/Add_an_External_Source.htm) for more information.

Lookup

Displays the name of the lookup table created in Target Design. The name
is a link that directs the user to further details about the lookup
table. Lookup tables can be viewed for mappings with any action. In
AutoGen, lookup tables are used with mappings that have an action of
RuleXref and Rule.

Target Relationship ID

Displays the name of the table that is joined to the current table in a
relationship. Relationships join Add Row and Update Row Sources
together. If the field is blank, then the Target for the selected
mapping is not joined to another.

**NOTE:** The relationship between an Add Row Source and an Update Row
Source that is external is auto derived.

Refer to [Add Relationship Joins to
Sources](../Use_Cases/Add_Relationship_Joins_to_Source.htm) for more
information.

Instruction

Displays the system-generated summary about the field mapping. If this
field is blank, the rule has not yet been autogenerated.

Additional Notes

Displays user-entered notes about the mapping.

Rule Where Clause

Displays the Where Clause used to filter the records to which a rule is
applied. The clause must consist of a column name, an operator and a
value. For example, Active = '1'. Refer to [Register Rules to
Tables](../../../Platform/Collect/Use_Cases/Add_Rules_and_Indices_to_Tables.htm#Register_Rules_to_Tables)
for more information.

Remediation Value

Displays the value to use while building a remediation report for field
mappings that do not use the Xref or RuleXref action.

**NOTE:** This field only displays when the Source is {Target Rules} .

Remediation Comment

Displays the remediation comment that display on the remediation report
for field mappings that do not use the Xref or RuleXref action. This
field only displays when {Target Rules} is selected on the
<span style="font-style: italic;">Field Mappings</span> page.

Rule Details

Generate Rule

If checked, the rule for the field is auto-generated.

Rule Name

Displays the name of the rule to be generated. This field only displays
when {Target Rules} is selected on the
<span style="font-style: italic;">Field Mappings</span> page.

 

## <span id="Audit_Information_tab"></span>Audit Information tab

Field

Description

Tracking

Mapped By

Displays user ID of individual who set the mapping to a MAPPING STATUS
of Complete. After a mapping status is set to Complete the mapping can
be submitted for approval.

Mapped On

Displays date and time when field mapping completed, as in when MAPPING
STATUS was set to Complete.

Submitted By

Displays user ID of individual who clicked Submit for the mapping on the
*Field Mappings* page. The mapping can then be approved or rejected on
the Mapping Approval page.

Submitted On

Displays date and time when the user clicked Submit for the mapping on
the *Field Mappings* page.

Created By

Displays user ID of individual who clicked the Create and Approve Rules
icon on the Automation page to create the rules for the approved
mapping.

Created On

Displays date and time when a user clicked the Create and Approve

Rules icon on the Automation page to create the rules for the approved
mapping.

Approved By

Displays user ID of individual who approved the mapping on the Mapping
Approval page. Once approved, the rules for the mapping can be created
on the Automation page

Approved On

Displays date and time when the mapping was approved on the Mapping
Approval page.

Rejected By

Displays user ID of individual who rejected the mapping on the Mapping
Approval page. If Rejected, the mapping must be updated and submitted
again on the *Field Mappings* page.

Rejected On

Displays date and time when the mapping was rejected on the Mapping
Approval page.
