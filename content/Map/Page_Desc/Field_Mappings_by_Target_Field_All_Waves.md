+++
title = 'Field Mappings by Target Field (All Waves)'
solution = 'Migration'
+++

# Field Mappings by Target Field (All Waves)

[Field Mappings by Target Field (All Waves)
V](#Field_Mappings_by_Target_Field__All_Waves__V)

<div class="use">

Use this page to [Copy a Mapping](../Use_Cases/Copy_a_Mapping).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Select <span style="font-weight: bold;">Map </span>in the Context
    bar.

3.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the [Process Area Launch](Process_Area_Launch_map) page.
    
    Or
    
    Click the <span style="font-weight: bold;">Targets</span> icon and
    click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.

4.  Click the <span style="font-weight: bold;">Mappings</span> icon for
    a Target or Target Source.

5.  Select a mapping.

6.  Click the <span style="font-weight: bold;">View All Waves
    Mappings</span> icon in the Page toolbar.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Copy</p></td>
<td><p>Click to copy the selected mapping to the selected Target or Source.</p>
<p><strong>NOTE:</strong> If more than one mapping is selected, this icon is disabled.</p>
<p><strong>NOTE:</strong> If the current user is a member of the Map WebApp Groups Ready Only or ValueMapper and is not a member of other groups with broader authorization for changes, this icon does not display.</p>
<p><strong>NOTE:</strong> If the selected field has an action set, the Copy icon is disabled. Fields with an action cannot be copied.</p></td>
</tr>
<tr class="odd">
<td><p>Wave Process Area</p></td>
<td><p>Displays the Wave and Process Area that contains the mapping for the field. All mappings across all Waves, Process Areas, and Objects for this field (based on System Types) display on this page.</p></td>
</tr>
<tr class="even">
<td><p>OBJECT</p></td>
<td><p>Displays the Object that contains the mapping for the field. All mappings across all Waves, Process Areas and Objects for this field (based on System Types) display on this page.</p></td>
</tr>
<tr class="odd">
<td><p>METRIC GROUP</p></td>
<td><p>Displays the name of the Metric Group added in Target Design Metric groups are a category of field groups that organize and prioritize fields in field groups for mapping.</p></td>
</tr>
<tr class="even">
<td><p>FIELD GROUP</p></td>
<td><p>Displays the name of the field group filter used to organize fields into subsets so that different rules, criticality levels, requirements settings and documentation can be set for these subsets based on values in related fields.</p></td>
</tr>
<tr class="odd">
<td><p>TARGET FIELD</p></td>
<td><p>Displays the name of the field to be mapped. The technical field name (including the table) is in bold. The field description is in italics.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE DETAILS</p></td>
<td><p>Displays the Source system name and the Add Row Source.</p>
<p>If the Source System says “SELECT SOURCE,” no Source has been selected. If it says “{Target Rules},” the rule is a Target rule.</p>
<p><strong>NOTE:</strong> If the Target field is a key field on the Target table, a key icon displays to the right of the field name.</p></td>
</tr>
<tr class="odd">
<td><p><span id="Mapping Actions" class="popUpLink">ACTION</span></p></td>
<td><p>Displays action used to map field.</p>
<p><strong>NOTE:</strong> If the selected field has an action (as in, a selection displays in the ACTION column), the Copy icon is disabled. Fields with an action cannot be copied.</p>
<p> Values are:</p>
<ul>
<li><a href="../Use_Cases/Construction">Construction</a></li>
<li><a href="../Use_Cases/Copy_Map">Copy</a></li>
<li><a href="../Use_Cases/Default_Action">Default</a></li>
<li><a href="../Use_Cases/Internal">Internal</a></li>
<li><a href="../Use_Cases/Manual_Rule">Manual Rule</a></li>
<li><a href="../Use_Cases/Manual_Construction">Manual Construction</a></li>
<li><a href="../Use_Cases/Not_Used">Not Used</a></li>
<li><a href="../Use_Cases/Rule">Rule</a></li>
<li><a href="../Use_Cases/Rule_Xref">Rule Xref</a></li>
<li><a href="../Use_Cases/Xref">Xref</a></li>
</ul>
<p>Refer to <a href="../Use_Cases/Perform_Field_Mapping#Select_an_Action">Select an Action</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>LOOKUP</p></td>
<td><p>Displays the name of the lookup table created in Target Design. Lookup tables can be viewed for mappings with any action. In AutoGen, lookup tables are used with mappings that have an action of RuleXref and Rule.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE TABLE</p></td>
<td><p>Displays Source table used for Copy, RuleXref, Xref or Construction actions.</p>
<p><strong>NOTE:</strong> When mapping a Source, this field displays the Add Row and Update Row Sources for the Add Row Source only. When mapping a Target, the field displays any Target in the Wave and Process Area.</p></td>
</tr>
<tr class="even">
<td><p>RULES COMMENT</p></td>
<td><p>Displays technical information entered by the Mapper to help the Developer build the rule when the action for the mapping is Manual Rule.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE FIELD</p></td>
<td><p>Displays Source field used for Copy, RuleXref, Xref or Construction actions.</p></td>
</tr>
<tr class="even">
<td><p>DEFAULT VALUE</p></td>
<td><p>Displays data used in the default rule creation process (as in, when ACTION is set to Default). For ACTIONS other than Default, this field is &lt;Blank&gt;.</p>
<p>While mapping a field with the Default action, a user can create output values for blank, empty, and null values.</p>
<p>The rule created by the mapping uses these output values:</p>
<ul>
<li>If the user enters &lt;blank&gt; in the Default field on the <span style="font-style: italic;"><a href="Field_Mappings_H">Field Mappings</a></span> page, the output used in the rule is single quotes with one space between them (' '). </li>
<li>If the user enters &lt;empty&gt;, the rule uses single quotes with no space between them ('').</li>
<li>If the user enters &lt;null&gt;, the rules uses NULL, representing no data.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>RULE SQL</p></td>
<td><p>Displays the SQL for the rule entered on the Mapping Approvals page. A developer must enter SQL when rejecting a mapping that has a Manual, Rule or RuleXref action.</p></td>
</tr>
<tr class="even">
<td><p>MAPPING STATUS</p></td>
<td><p>Displays an icon that represent  the <span id="Mapping Status" class="popUpLink"> Mapping Status</span> of the field in the mapping process.</p>
<ul>
<li>A red icon indicates a Mapping Status of Pending Review.</li>
<li>A yellow icon represents Design Required.</li>
<li>A green icon indicates mapping is Complete.</li>
</ul>
<p>A user can update the Mapping Status on the <span style="font-style: italic;">Vertical</span> View.</p></td>
</tr>
<tr class="odd">
<td><p>RULE STATUS</p></td>
<td><p>Displays an icon representing the <span id="Rule Status" class="popUpLink">Rule Status</span> of the rule to be built from the mapping once it is complete.</p>
<ul>
<li>A red icon indicates a Rule Status of Pending Review.</li>
<li>A yellow icon represents Revision Requested or that the associated mapping has been submitted and is waiting for Developer review.</li>
<li>A green icon indicates the Rule is Complete.</li>
</ul>
<p>Rule status is updated by the system and cannot be changed by the user in Map.</p>
<p>Rule status can be updated in SQL AutoGen on the <a href="../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H">Automation SQL Field Mappings</a> page. Refer to <a href="../../SQL_AutoGen/Use_Cases/Update_a_Rule_Status">Update a Rule Status</a> for more information.  </p></td>
</tr>
</tbody>
</table>

## <span id="Field_Mappings_by_Target_Field__All_Waves__V"></span>Field Mappings by Target Field (All Waves) V

[Field Mappings by Target Field (All Waves)
H](Field_Mappings_by_Target_Field_All_Waves)

<div class="use">

Use this page to view information about the field mapping.

</div>

This page has the following tabs:

  - [General](#General_tab)
  - [Audit Information](#Audit_Information_tab)

## <span id="General_tab"></span>General tab

Field

Description

Status

Mapping Status

Displays an icon that represents  the
<span id="Mapping Status" class="popUpLink">Mapping Status</span> of the
field in the mapping process.

Rule Status

Displays an icon representing the
<span id="Rule Status" class="popUpLink">Rule Status</span> of the rule
to be built from the mapping once it is complete.

Rule status is updated by the system and cannot be changed by the user
in Map.

Rule status can be updated in SQL AutoGen on the[*Automation SQL Field
Mappings*](../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H)
page. Refer to [Update a Rule
Status](../../SQL_AutoGen/Use_Cases/Update_a_Rule_Status) for more
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

**NOTE:** This list box displays Update Row Sources only. An Add Row
Source cannot be used as an External Source type. The External Source
table must be registered as an Update Row first.

Refer to [Add an External
Source](../Use_Cases/Add_an_External_Source) for more information.

Lookup

Displays the name of the lookup table created in Target Design. Lookup
tables can be viewed for mappings with any action. In AutoGen, lookup
tables are used with mappings that have an action of RuleXref and Rule.

Target Relationship ID

Displays the name of the table that is joined to the current table in a
relationship. Relationships join Add Row and Update Row Sources
together. If the field is blank, then the Target for the selected
mapping is not joined to another.

Instruction

Displays the system-generated summary about the field mapping.

Remediation Value

Displays the value to use while building a remediation report for field
mappings that do not use the Xref or RuleXref action. This field only
displays when {Target Rules} is selected on the
<span style="font-style: italic;">[Field
Mappings](Field_Mappings_H)</span> page. This field only displays
for {Target Rule} Target Sources.

Remediation Comment

Displays the remediation comment that display on the remediation report
for field mappings that do not use the Xref or RuleXref action. This
field only displays when {Target Rules} is selected on the
<span style="font-style: italic;">[Field
Mappings](Field_Mappings_H)</span> page.

Additional Notes

Displays user-entered notes about the mapping.

Where Clause Override

The Where Clause Override is an extra clause that conditions to the
download SQL, for example, WHERE SPRSL NOT IN (‘a’,’b’,’c’,’d’) and
Where ColumnKey like ‘2007%’.

**NOTE**: When a where clause override is added to a table that is set
up as a Data Services package the initial build will require an
additional build. Immediately after the first build runs, the user must
rerun the build. The second build will use the clause entered in the
Where Clause Override field to refresh the table’s contents when a
refresh is run. After the second build, the clause entered in the Where
Clause Override field will be up to date for every subsequent build, and
the user is not required to build the package more than once.

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
the *Mapping Approval* page.

Submitted On

Displays date and time when the user clicked Submit for the mapping on
the *Field Mappings* page.

Created By

Displays user ID of individual who clicked the Create and Approve Rules
icon on the
<span style="font-style: italic;">[Automation](../../SQL_AutoGen/Page_Desc/Automation_page)</span>
page or the Create and Complete icon on the [Automation SQL Field
Mappings](../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H)
page  to create the rules for the approved mapping.

Created On

Displays date and time when a user clicked the Create and Approve Rules
icon on the
<span style="font-style: italic;">[Automation](../../SQL_AutoGen/Page_Desc/Automation_page)</span>
page or the Create and Complete icon on the [Automation SQL Field
Mappings](../../SQL_AutoGen/Page_Desc/Automation_SQL_Field_Mappings_H)
page  to create the rules for the approved mapping.

Approved By

Displays user ID of individual who approved the mapping on the *Mapping
Approval* page. Once approved, the rules for the mapping can be created
on the Automation page

Approved On

Displays date and time when the mapping was approved on the *[Mapping
Approval](Mapping_Approval_H)* page.

Rejected By

Displays user ID of individual who rejected the mapping on the *Mapping
Approval* page. If Rejected, the mapping must be updated and submitted
again on the *Field Mappings* page.

Rejected On

Displays date and time when the mapping was rejected on the *Mapping
Approval* page.
