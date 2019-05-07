+++
title = 'Object Field Groups'
solution = 'Migration'
+++

# Object Field Groups

<div class="use">

Use this page to [Assign a Field Group to an
Object](../Use_Cases/Assign_a_Field_Group_to_an_Object.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Select <span style="font-weight: bold;">Design </span>in the Context
    bar.
3.  Select <span style="font-weight: bold;">Configuration \> Field Group
    Setup</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>OBJECT ID</p></td>
<td><p>Displays the Object that contains the field group that can be applied to that Object’s Targets.</p>
<p>Objects are added in Console. Refer to <a href="../../Console/Use_Cases/Add_Elements_Separately.htm#Add3">Add an Object</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>FIELD GROUP ID</p></td>
<td><p>Displays the name of the field group filter assigned to the Object, used to organize fields into subsets so that different rules, criticality levels, requirements settings, and documentation can be set for these subsets based on values in related fields. Target Design is delivered with a default field group (*) to which every field belongs.</p>
<p>The Field Group is added on the <span style="font-style: italic;"><a href="Field_Groups.htm">Field Groups</a></span> page.</p>
<p>Refer to <a href="../Use_Cases/Create_Field_Groups.htm">Create Field Groups</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>RULE PRIORITY OFFSET</p></td>
<td><p>Displays a number (always negative) that is subtracted from the rule’s priority to set the order the rule is run.</p>
<p><strong>NOTE</strong>: The default field group (*) displays 0. This feature cannot be used for the default field group.</p>
<p><strong>NOTE</strong>: If this field is blank when the record is saved, the default value -1 is added to the field.</p>
<p>Refer to <a href="../Use_Cases/Set_Rule_Priority_for_Fields_in_Field_Groups.htm">Set Rule Priority for Fields in Field Groups</a> for more information.</p></td>
</tr>
</tbody>
</table>
