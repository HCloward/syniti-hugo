+++
title = 'Field Mapping History'
solution = 'Migration'
+++

# Field Mapping History

<div class="use">

Use this page to:

  - [View Field Mapping
    History](../Use_Cases/View_Field_Mapping_History)
  - [Restore Current Field Mapping From
    History](../Use_Cases/Restore_Current_Field_Mapping_From_History)

</div>

To access this page in dspMigrate:

1.  Select <span style="font-weight: bold;">Map </span> <span>in the
    Context bar.</span>
2.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area Launch](Process_Area_Launch_map)* page.
3.  Click the <span style="font-weight: bold;">Mappings</span> icon for
    a Target.
4.  Select a field and click the
    <span style="font-weight: bold;">History</span> icon in the Page
    toolbar.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Restore</p></td>
<td><p>Click to restore the current mapping for a field to the selected field history mapping.</p>
<p>This defaults the current mapping to a Rule Status of Pending Review.</p></td>
</tr>
<tr class="odd">
<td><p>ID</p></td>
<td><p>Displays unique identifier assigned to each history record.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE</p></td>
<td><p>Displays the Source database that contains the data to be migrated to the Target.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE DATABASE OBJECT</p></td>
<td><p>Displays the Source table name containing fields that will be mapped to the Target table.</p></td>
</tr>
<tr class="even">
<td><p>TARGET</p></td>
<td><p>Displays the Target table name.</p></td>
</tr>
<tr class="odd">
<td><p>FIELD GROUP</p></td>
<td><p>Displays the field group that the field belongs to. Field groups are assigned to fields in Target Design and allow mappings to be applied using filters based on the values in another table.</p></td>
</tr>
<tr class="even">
<td><p>FIELD</p></td>
<td><p>Displays name of the field to be mapped.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays description of the field (from the Source table) to be mapped.</p></td>
</tr>
<tr class="even">
<td><p>INSTRUCTION</p></td>
<td><p>Displays the system-generated summary about the field mapping.</p></td>
</tr>
<tr class="odd">
<td><p>MAPPING STATUS</p></td>
<td><p>Displays the <span id="Mapping Status" class="popUpLink">Mapping Status</span> of the field in the mapping process.</p></td>
</tr>
<tr class="even">
<td><p>MAPPED BY</p></td>
<td><p>Displays the user name of the user who selected Complete in the Mapping Status list box on the <span style="font-style: italic;"><a href="Field_Mappings_H">Field Mappings</a></span> page.</p></td>
</tr>
<tr class="odd">
<td><p>MAPPED ON</p></td>
<td><p>Displays the date and time the user selected Complete on the <span style="font-style: italic;">Field Mappings</span> page for a mapping.</p></td>
</tr>
<tr class="even">
<td><p>SUBMITTED BY</p></td>
<td><p>Displays the user ID of the user who clicked Submit on the Field Mappings page to submit the mapping for approval and for automation.</p></td>
</tr>
<tr class="odd">
<td><p>SUBMITTED ON</p></td>
<td><p>Displays the date and time the user clicked Submit.</p></td>
</tr>
<tr class="even">
<td><p>APPROVED BY</p></td>
<td><p>Displays the user ID of the Developer who approved the mapping on the <em><a href="Mapping_Approval_H">Mapping Approval</a></em> page.</p></td>
</tr>
<tr class="odd">
<td><p>APPROVED ON</p></td>
<td><p>Displays the date and time the Developer approved the mapping on the <em>Mapping Approval</em> page.</p></td>
</tr>
<tr class="even">
<td><p>REJECTED BY</p></td>
<td><p>Displays the user ID of the Developer who rejected the mapping on the <em>Mapping Approval</em> page.</p></td>
</tr>
<tr class="odd">
<td><p>REJECTED ON</p></td>
<td><p>Displays the date the Developer rejected the mapping on the <em>Mapping Approval</em> page.</p></td>
</tr>
<tr class="even">
<td><p><span id="Mapping Actions" class="popUpLink">ACTION</span></p></td>
<td><p>Displays mapping action at the time when MAPPING STATUS was set to Complete on the <em>Field Mappings</em> page.</p></td>
</tr>
<tr class="odd">
<td><p>DEFAULT VALUE</p></td>
<td><p>Displays default value at the time when MAPPING STATUS was set to Complete on the <em>Field Mappings</em> page.</p>
<p>A default value is required with the Default action only. The default action is used when mapping a field that should write a default value to the Target field.</p>
<p>While mapping a field with the Default action, a user can create output values for blank, empty, and null values. The rule created by the mapping uses these output values. If the user enters &lt;blank&gt; in the Default field on the Field Mappings page, the output used in the rule is single quotes with one space between them (' '). If the user enters &lt;empty&gt;, the rule uses single quotes with no space between them (''). If the user enters &lt;null&gt;, the rules uses NULL, representing no data.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE TABLE</p></td>
<td><p>Displays Source table name required for an action of Copy, RuleXref or Xref.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE FIELD</p></td>
<td><p>Displays Source field name required for an action of Copy, RuleXref or Xref.</p></td>
</tr>
<tr class="even">
<td><p>METRIC GROUP</p></td>
<td><p>Displays the metric group name.</p>
<p>Metric groups are added in Target Design and are a subcategory of field groups. They prioritize and organize fields in field groups for mapping.</p>
<p>Refer to <a href="../../Design/Use_Cases/Work_with_Metric_Groups">Work with Metric Groups</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>CHECK TABLE</p></td>
<td><p>Displays Check Table assigned at the time when MAPPING STATUS was set to Complete on the <em>Field Mappings</em> page.</p></td>
</tr>
<tr class="even">
<td><p>AUTO GENERATE RULE</p></td>
<td><p><span>If checked, AutoGen generated a SQL rule for this mapping.</span></p></td>
</tr>
<tr class="odd">
<td><p>REMEDIATION VALUE</p></td>
<td><p>Displays the value to use while building a remediation report for field mappings that do not use the Xref or RuleXref action. This field only displays when {Target Rules} is selected on the <em>Field Mappings</em> page.</p></td>
</tr>
<tr class="even">
<td><p>REMEDIATION COMMENT</p></td>
<td><p>Displays the remediation comment that displays on the remediation report for field mappings that do not use the Xref or RuleXref action. This field only displays when {Target Rules} is selected on the <em>Field Mappings</em> page.</p></td>
</tr>
<tr class="odd">
<td><p>RULE STATUS</p></td>
<td><p>Displays the <span id="Rule Status" class="popUpLink">Rule Status</span> of the rule to be built from the mapping once it is complete.</p></td>
</tr>
<tr class="even">
<td><p>RULES COMMENT</p></td>
<td><p>Displays technical information entered by the Mapper to help the Developer build the rule when the action for the mapping is Manual Rule.</p></td>
</tr>
<tr class="odd">
<td><p>ADDITIONAL NOTES</p></td>
<td><p>Displays notes about the mapping.</p></td>
</tr>
<tr class="even">
<td><p>RULE SQL</p></td>
<td><p>Displays the SQL for the rule entered by the Developer on the <span style="font-style: italic;">Mapping Approval</span> page or by the Mapper on the <span style="font-style: italic;">Vertical</span> View of the <span style="font-style: italic;">Field Mappings</span> page.</p></td>
</tr>
</tbody>
</table>
