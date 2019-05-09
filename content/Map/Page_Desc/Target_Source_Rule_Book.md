+++
title = 'Target Source Rule Book'
solution = 'Migration'
+++

# Target Source Rule Book

<div class="use">

Use this page to [View All Mappings for a
Target](../Use_Cases/View_all_Mappings_for_a_Target).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Map </span>in the Context
    bar.
3.  Click the <span style="font-weight: bold;">Metrics</span> icon on
    the *[Process Area Launch](Process_Area_Launch_map)* page.
4.  Click the <span style="font-weight: bold;">Rule Book</span> icon on
    the *[Metrics and Reports Landing](Metrics_and_Reports_Landing)*
    page.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the name of the object as created in Console.</p></td>
</tr>
<tr class="odd">
<td><p>TARGET</p></td>
<td><p>Displays the Target table name.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE</p></td>
<td><p>Displays the Source name.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE DATABASE OBJECT_TARGET RULE</p></td>
<td><p>Displays the type of rule for the mapping.</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays order in which Target field is run in the Transform rule.</p></td>
</tr>
<tr class="odd">
<td><p>FIELD GROUP</p></td>
<td><p>Displays current field group to which the selected field belongs. Field groups are assigned in Target Design, and allow users to apply filters for mapping based on certain values in a field. Refer to <a href="../../Design/Use_Cases/Work_with_Field_Groups">Work with Field Groups</a>   for more information.</p></td>
</tr>
<tr class="even">
<td><p>FIELD</p></td>
<td><p>Displays the Source field to be mapped to the Target field</p></td>
</tr>
<tr class="odd">
<td><p>CHECK TABLE</p></td>
<td><p>Displays the check table name if the field mapping must be value mapped.</p></td>
</tr>
<tr class="even">
<td><p>MAPPING STATUS</p></td>
<td><p>Displays the <span id="Mapping Status" class="popUpLink">Mapping Status</span> of the field in the mapping process.</p></td>
</tr>
<tr class="odd">
<td><p>RULE STATUS</p></td>
<td><p>Displays the <span id="Rule Status" class="popUpLink">Rule Status</span> of the rule to be built from the mapping once it is complete.</p></td>
</tr>
<tr class="even">
<td><p>ACTION</p></td>
<td><p>Displays the <span id="Mapping Actions" class="popUpLink">Mapping Action</span> assigned to the field mapping, such as Copy, Default, or Rule.</p></td>
</tr>
<tr class="odd">
<td><p>DEFAULT VALUE</p></td>
<td><p>Displays the default value to be inserted in the Target field if the Action is Default for the field mapping.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE TABLE</p></td>
<td><p>Displays the Source table that stores the Source field to be mapped to the Target field.</p>
<p>This field is used with the Copy, RuleXref and Xref actions.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE FIELD</p></td>
<td><p>Displays the Source field to be mapped to the Target field.</p>
<p>This field is used with the Copy, RuleXref and Xref actions.</p></td>
</tr>
<tr class="even">
<td><p>RULES COMMENT</p></td>
<td><p>Displays technical information entered by the Mapper to help the Developer build the rule when the action for the mapping is Manual Rule.</p></td>
</tr>
<tr class="odd">
<td><p>INSTRUCTION</p></td>
<td><p>Displays the system-generated summary about the field mapping</p></td>
</tr>
<tr class="even">
<td><p>RULE SQL</p></td>
<td><p>Displays the SQL for the rule entered on the <em><a href="Mapping_Approval_H">Mapping Approval</a></em> page. A developer must enter SQL when rejecting a mapping that has a Manual, Rule or RuleXref action .</p></td>
</tr>
<tr class="odd">
<td><p>RULE WHERE CLAUSE</p></td>
<td><p>Displays the Where Clause used to filter the records to which a rule is applied. The clause must consist of a column name, an operator and a value. For example, Active = '1 '.</p></td>
</tr>
<tr class="even">
<td><p>COMMENT</p></td>
<td><p>Displays the comment entered by the Developer on the <em>Mapping Approval</em>page when reviewing the mapping.</p></td>
</tr>
<tr class="odd">
<td><p>MAPPED BY</p></td>
<td><p>Displays the user name of the Mapper who set the mapping status.</p></td>
</tr>
<tr class="even">
<td><p>MAPPED ON</p></td>
<td><p>Displays the date the MAPPING STATUS was set to Complete on the <em><a href="Field_Mappings_H">Field Mappings</a></em> page for the mapping.</p></td>
</tr>
<tr class="odd">
<td><p>CREATED ON</p></td>
<td><p>Displays the date the rule was created.</p></td>
</tr>
<tr class="even">
<td><p>CREATED BY</p></td>
<td><p>Displays the user name of the user who clicked Create or Create All Rules in AutoGen.</p></td>
</tr>
<tr class="odd">
<td><p>APPROVED BY</p></td>
<td><p>Displays the name of the Developer who approved the mapping on the <em><a href="Mapping_Approval_H">Mapping Approval</a></em> page.</p></td>
</tr>
<tr class="even">
<td><p>APPROVED ON</p></td>
<td><p>Displays the date the mapping was approved.</p></td>
</tr>
<tr class="odd">
<td><p>Wave NAME</p></td>
<td><p>Displays the Wave name for the current context created in Console.</p></td>
</tr>
<tr class="even">
<td><p>Process Area</p></td>
<td><p>Displays the Process Area name for the current context created in Console.</p></td>
</tr>
<tr class="odd">
<td><p>ERP TABLE NAME</p></td>
<td><p>Displays the name of the ERP Target table that stores the Target field to be mapped.</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays the description of the Target field in the ERP system.</p></td>
</tr>
<tr class="odd">
<td><p>METRIC GROUP</p></td>
<td><p>Displays the metric group name.</p>
<p>Metric groups are added in Target Design and are a subcategory of field groups. They prioritize and organize fields in field groups for mapping.</p>
<p>Refer to <a href="../../Design/Use_Cases/Work_with_Metric_Groups">Work with Metric Groups</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>KEY FIELD</p></td>
<td><p>If checked, the rule is a key, or primary field, on the table.</p></td>
</tr>
<tr class="odd">
<td><p>HELP TEXT</p></td>
<td><p>Displays help text provided by the Source system.</p></td>
</tr>
<tr class="even">
<td><p>DATA TYPE</p></td>
<td><p>Displays the data type of the field in the Target system.</p></td>
</tr>
<tr class="odd">
<td><p>LENGTH</p></td>
<td><p>Displays the length of the field in the Target system.</p></td>
</tr>
<tr class="even">
<td><p>DECIMALS</p></td>
<td><p>Displays the number of decimal places allowed for a value in the Target field.</p></td>
</tr>
</tbody>
</table>
