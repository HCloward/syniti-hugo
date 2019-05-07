+++
title = 'Wave Compare for Target Field Results H'
solution = 'Migration'
+++

# Wave Compare for Target Field Results H

[Wave Compare for Target Field Results
V](Wave_Compare_for_Target_Field_Results.htm#Wave_Compare_for_Target_Field_Results_V)

<div class="use" data-xmlns="">

Use this page to [Synchronize Target Designs Across
Waves](../Use_Cases/Synchronize_Target_Designs_Across_Waves.htm).

</div>

**NOTE**: This page is only accessible if the current user is a member
of the WebApp group Wavesynchronizer in Console or is assigned to a
security role with access to the page. Refer to [Set
Security](../../../Platform/Sys_Admin/Use_Cases/Setting_security.htm) in
System Administration for more information.

To access this page:

1.  Select
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">dspMigrate</span>
    in the
    <span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">Navigation</span>
    pane, or select
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Console</span>
    in the Context bar.
2.  Click
    the<span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">
    Build Comparison</span> icon in the Page toolbar.
3.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Fields
    </span>icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Hide Identical</p></td>
<td><p><span style="font-family: Arial, sans-serif;">Click to hide or unhide</span> all matching comparisons in the Target  fields (as in, those comparisons that do not need to be synced) to make comparisons easier to review.</p></td>
</tr>
<tr class="odd">
<td><p>Sync Field</p></td>
<td><p>Click to sync the Target design for the selected field between the child Wave and the baseline Wave.</p></td>
</tr>
<tr class="even">
<td><p>Sync All Fields</p></td>
<td><p>Click to sync the Target design for all fields between the child Wave and the baseline Wave.</p></td>
</tr>
<tr class="odd">
<td><p>Process Area</p></td>
<td><p>Displays the Process Area in the child Wave that has been compared to the baseline Wave.</p></td>
</tr>
<tr class="even">
<td><p>OBJECT</p></td>
<td><p>Displays the Object in the child Wave that has been compared to the baseline Wave.</p></td>
</tr>
<tr class="odd">
<td><p>TARGET</p></td>
<td><p>Displays the name of the Target.</p></td>
</tr>
<tr class="even">
<td><p>FIELD NAME</p></td>
<td><p>Displays the field name (for example, MANDT).</p></td>
</tr>
<tr class="odd">
<td><p>FIELD ORDER</p></td>
<td><p>Displays the order of the field entered on the <em><a href="../../Design/Page_Desc/Target_Fields_H_Target_Design.htm">Target Fields</a></em> page.</p></td>
</tr>
<tr class="even">
<td><p>LABEL</p></td>
<td><p>Displays the user friendly name for the field (for example, Client).</p></td>
</tr>
<tr class="odd">
<td><p>FIELD GROUP</p></td>
<td><p>Displays the name of the field group to which the field belongs. All fields are assigned to the default field group (*). Field groups are used to organize data to be able to apply different rules, criticality levels, requirements settings against each group depending on the values of data in a related field..</p>
<p>Refer to <span style="font-family: Arial, sans-serif;color: #0000ff;"><a href="../../Design/Use_Cases/Work_with_Field_Groups.htm">Work With Field Groups</a></span> <span style="font-family: Arial, sans-serif;">for more information.</span></p></td>
</tr>
<tr class="even">
<td><p>KEY FIELD</p></td>
<td><p>If checked, the field is a key field on the table.</p></td>
</tr>
<tr class="odd">
<td><p>ACTIVE</p></td>
<td><p>If checked, the field is active and can be used for mapping. If disabled, the field cannot be used in mapping, and is not pushed to Map when the Target design is synced.</p></td>
</tr>
<tr class="even">
<td><p>TARGET LOOKUP TABLE</p></td>
<td><p>Displays the name of the lookup table to which a field belongs.</p>
<p>Refer to <span style="font-family: Arial, sans-serif;color: #0000ff;"><a href="../../Design/Use_Cases/Set_up_Lookup_Tables.htm">Set up Lookup Tables</a></span> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>DATA TYPE</p></td>
<td><p>Displays the field’s data type, such as NVARCHAR or DECIMAL</p>
<p><strong>NOTE</strong>: The data type of a field determines whether the Length and Decimal fields on this page are required. When the following data types are selected, the Length field is required:</p>
<ul>
<li>NVARCHAR</li>
<li>DECIMAL</li>
<li>NCHAR</li>
<li>NVARCHAR</li>
</ul>
<p>When the field’s data type is DECIMAL or DATETIME, the Decimal field is required. </p></td>
</tr>
<tr class="even">
<td><p>LENGTH</p></td>
<td><p>Displays the field length, or the maximum allowable characters/numbers that the field can store. This field is required when the field’s data type is:</p>
<ul>
<li>NVARCHAR</li>
<li>DECIMAL</li>
<li>NCHAR</li>
<li>NVARCHAR</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>REQUIRED</p></td>
<td><p>Displays the Requirement setting used for reporting. The platform is delivered with the following settings that cannot be edited or deleted.</p>
<ul>
<li><strong>Technical Required</strong> -The ERP System cannot run without a value.</li>
<li><strong>Business Required</strong> -The Business requires this field to have a value.</li>
<li><strong>Conditional Required</strong> - Based upon other field settings this field may or may not be required.</li>
<li><strong>Optional</strong> -This view is not required by ERP system or Business users.</li>
</ul></td>
</tr>
</tbody>
</table>

## <span id="Wave_Compare_for_Target_Field_Results_V"></span>Wave Compare for Target Field Results V

[Wave Compare for Target Field Results
H](Wave_Compare_for_Target_Field_Results.htm)

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Hide Identical</p></td>
<td><p>Click to hide or unhide all matching comparisons in the Target fields (as in, those comparisons that do not need to be synced) to make comparisons easier to review.</p></td>
</tr>
<tr class="odd">
<td><p>Process Area</p></td>
<td><p>Displays the Process Area in the child Wave that has been compared to the baseline Wave.</p></td>
</tr>
<tr class="even">
<td><p>Object</p></td>
<td><p>Displays the Object in the child Wave that has been compared to the baseline Wave.</p></td>
</tr>
<tr class="odd">
<td><p>Target</p></td>
<td><p>Displays the name of the Target.</p></td>
</tr>
<tr class="even">
<td><p>Field Group</p></td>
<td><p>Displays the name of the field group to which the field belongs. All fields are assigned to the default field group (*). Field groups are used to organize data to be able to apply different rules, criticality levels, requirements settings against each group depending on the values of data in a related field.</p>
<p>Refer to <span style="font-family: Arial, sans-serif;color: #0000ff;"><a href="../../Design/Use_Cases/Work_with_Field_Groups.htm">Work With Field Groups</a></span> <span style="font-family: Arial, sans-serif;">for more information.</span></p></td>
</tr>
<tr class="odd">
<td><p>Field Name</p></td>
<td><p>Displays the field name (for example, MANDT).</p></td>
</tr>
<tr class="even">
<td><p>Field Comparison</p></td>
<td><p>Displays a table that lists the fields in the baseline Wave and the child Wave and the differences between them for the selected field.</p></td>
</tr>
</tbody>
</table>
