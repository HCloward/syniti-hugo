+++
title = 'Field Groups'
solution = 'Migration'
+++

# Field Groups

<div class="use">

Use this page to [Create Field
Groups](../Use_Cases/Create_Field_Groups).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Select <span style="font-weight: bold;">Design </span>in the Context
    bar.
3.  Select <span style="font-weight: bold;">Configuration \> Field
    Groups</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>FIELD GROUP</p></td>
<td><p>Displays the name of the field group filter used to organize fields into subsets so that different rules, criticality levels, requirements settings and documentation can be set for these subsets based on values in related fields. Target Design is delivered with a default field group (*) .</p>
<p>The default field group cannot be updated or deleted.</p>
<p>Once added, the FIELD GROUP is an option on the <span style="font-style: italic;"><a href="Object_Field_Groups">Object Field Groups</a></span> page in the Field Group ID list box.</p>
<p><strong>NOTE</strong>: Naming each field group after the filter value it is based on is a good practice.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a user-entered description of the field group filter.</p>
<p><strong>NOTE</strong>: This field is blank for the (*) field group.</p></td>
</tr>
<tr class="even">
<td><p>FILTER TABLE</p></td>
<td><p>Displays the ERP Target table that contains the field and value used in the field group filter.</p>
<p><strong>NOTE</strong>: The default field group (*) displays * in the FILTER TABLE field, indicating that no filters are applied to the table (as in, all records are selected).</p></td>
</tr>
<tr class="odd">
<td><p>FILTER FIELD</p></td>
<td><p>Displays the ERP Target table field that contains the value used to define the criterion for the filter.</p>
<p><strong>NOTE</strong>: The default field group (*) displays * in the FILTER FIELD field, indicating that no filters are applied to fields in the table.</p></td>
</tr>
<tr class="even">
<td><p>FILTER VALUE</p></td>
<td><p>Displays the value of filter applied in the field group. For example, to filter on finished goods for SAP, FILTER TABLE = MARA, FIELD FIELD = MTART and FILTER VALUE = FERT.</p>
<p><strong>NOTE</strong>: The default field group (*) displays * in the FILTER VALUE field, indicating that no filters are applied to values in any fields.</p></td>
</tr>
<tr class="odd">
<td><p>RULE PRIORITY OFFSET</p></td>
<td><p>Displays a number (<span>always negative) that is subtracted from the rule’s priority to set the order the rule is run.</span></p>
<p>The default field group (*) displays 0. This feature cannot be used for the default field group.</p>
<p>Refer to <a href="../Use_Cases/Set_Rule_Priority_for_Fields_in_Field_Groups">Set Rule Priority for Fields in Field Groups</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>DSP SUPPLIED</p></td>
<td></td>
</tr>
</tbody>
</table>
