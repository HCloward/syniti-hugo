+++
title = 'System Types Mappings'
solution = 'Platform'
+++

# System Types Mappings

<div class="use">

Use this page to [Add Mappings](../Use_Cases/Add_Mappings.htm).

</div>

To access this page:

1.  Select **Common \> System Types** in the *Navigation* pane.
2.  Click the **Target Mappings** icon for a System Type.

<span style="font-weight: bold;">NOTE:</span> Excel Integration has been
enabled on this page. Refer to [Use Excel
Integration](../../Excel_Int/Use_Excel_Integration.htm) for more
information.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>SOURCE SYSTEM TYPE TABLE ID</p></td>
<td><p>Displays table within the target system being mapped.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays description of the mapping.</p></td>
</tr>
<tr class="even">
<td><p>TARGET SYSTEM TYPE TABLE FIELD ID</p></td>
<td><p>Displays table field within target system being mapped; fields are mapped from a source to a target system.</p></td>
</tr>
<tr class="odd">
<td><p>ACTION</p></td>
<td><p>Displays type of mapping. Options are:</p>
<ul>
<li><strong>Construction</strong> – Constructs data in Construct because source data does not exist for this Target ERP field.</li>
<li><strong>Copy</strong> – Copies the legacy value directly into the Target ERP system, unchanged.</li>
<li><strong>Cross Reference</strong> – Cross references the legacy value using value mapping to convert the source value to a Target ERP value.</li>
<li><strong>Default</strong> – Defaults all records to value in DEFAULT VALUE field.</li>
<li><strong>Internal</strong> – Generates number inside Legacy system as the record is loaded, which is typically the key value.</li>
<li><strong>Manual Construction</strong> – Indicates a rule that will be built manually in Construct</li>
<li><strong>Manual Rule</strong> – Creates rule using provided SQL code.</li>
<li><strong>Not Used</strong> – No mapping is required because the field will not be loaded into the Target ERP system.</li>
<li><strong>Rule</strong> – Creates a rule for complex field mapping. Any action that is too complex for a Default, Copy or Cross Reference.</li>
<li><strong>Rule Cross Reference</strong> – Performs manipulation of the source value and then converts the value to a Target ERP value using value mapping.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>RULE SQL</p></td>
<td><p>Displays SQL used to generate the rule if the action is Manual Rule.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE SYSTEM TYPE TABLE FIELD ID</p></td>
<td><p>Displays table field within the source system being mapped; fields are mapped from a source to a target system.</p></td>
</tr>
<tr class="even">
<td><p>RULE COMMENT</p></td>
<td><p>Displays information about the rule.</p></td>
</tr>
<tr class="odd">
<td><p>DEFAULT VALUE</p></td>
<td><p>Displays the mapping value used for an Action of Default.</p></td>
</tr>
<tr class="even">
<td><p>RULE TYPE</p></td>
<td><p>Displays the value <span style="font-size: 11.0pt;font-family: Arial, sans-serif;">to determine the rule category to import mappings. The options are</span>SourceRule or TargetRule.</p></td>
</tr>
<tr class="odd">
<td><p>MAPPING GROUP ID</p></td>
<td><p>Displays name of mapping group.</p></td>
</tr>
<tr class="even">
<td><p>FIELD GROUP</p></td>
<td><p>Displays field group used to further categorize the fields in mappings. Field groups do not impact rule generation.</p></td>
</tr>
<tr class="odd">
<td><p>MAPPING SET ID</p></td>
<td><p>Displays the Mapping Set to which the Mapping is assigned. The Mapping Set can be used to logically group several Mapping records.</p></td>
</tr>
<tr class="even">
<td><p>SYSTEM TYPE JOIN ID</p></td>
<td><p>Displays the name of the join added on the <a href="System_Types_Joins.htm">System Types Joins</a> page.</p>
<p><strong>NOTE:</strong> Table join relationships indicate how table fields are connected; they must be manually added to System Types.</p></td>
</tr>
<tr class="odd">
<td><p>DSP SUPPLIED</p></td>
<td><p>If checked, this content is installed with the platform and cannot be edited.</p>
<p>If unchecked, the content was added by a user or process.</p>
<p><strong>NOTE:</strong> This is a display-only check box. It cannot be updated.</p></td>
</tr>
</tbody>
</table>
