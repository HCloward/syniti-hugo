+++
title = 'Naming Conventions'
solution = 'Migration'
+++

# Naming Conventions

BackOffice follows a very strict naming convention that provides a
methodology for creating names that each member of the team can
understand.

Every table has two names: informal and formal. Use the informal table
name, such as MARC or MARA when naming objects.  Use the formal table
name, such as ttMARC or ttMARA, when naming a Target rule.

Use the naming convention:

tr\[InformalTableName\]\_\[FieldName\]\_Sel, displayed as:
trMARA\_MAKTXUpdSel.

The formal table name for this table is ttMAKT. Note that the informal
table naming convention in this example does not produce
trttMAKT\_MAKTXUpdSel, rather it should produce the following name
trMAKT\_MAKTXUpdSel. This informal table name rule is also used when
naming Source rules, Source/Target reports and Target exports.

Refer to the following table for the standard naming conventions to use
throughout Transform.

<table>
<tbody>
<tr class="odd">
<td><p>Item</p></td>
<td><p>Naming Convention</p></td>
</tr>
<tr class="even">
<td><p>Source System ID</p></td>
<td><p>[Source System Name]_[Location]</p>
<p><strong>NOTE:</strong> Location is optional.</p></td>
</tr>
<tr class="odd">
<td><p>Source Report</p></td>
<td><p>sv[InformalTableName]_[FieldName]_[Description]Sel</p></td>
</tr>
<tr class="even">
<td><p>Sub-View for Source Reports</p></td>
<td><p>sv[InformalTableName]_[FieldName]_[AdditionalActionDescription][010]Sel or</p>
<p>sv[InformalTableName]_[FieldName]_[AdditionalActionDescription][020]Sel</p></td>
</tr>
<tr class="odd">
<td><p>Source Table</p></td>
<td><p>st[TargetTableName]_[SourceSystemID]_[SourceTableName]</p></td>
</tr>
<tr class="even">
<td><p>Source Repository</p></td>
<td><p>sdb[Source SystemID]</p></td>
</tr>
<tr class="odd">
<td><p>Source Rule</p></td>
<td><p>View: sr[InformalTableName]_[FieldName]UpdSel</p>
<p>Stored Procedure:  sr[InformalTableName]_[FieldName]Upd</p>
<p>If Field Groups are being used:</p>
<p>View: sr[InformalTableName]_[FieldName]_[FieldGroup]UpdSel</p>
<p>Stored Procedure: Sr[InformalTableName]_[FieldName]_[FieldGroup]Upd</p>
<p> </p>
<p>If Field Groups are being used:</p>
<p>For Manual Rules (System won’t generate a namespace for these):</p>
<p>View: sr[InformalTableName]_[FieldName]_[FieldGroup]_[AdditionalDescription]UpdSel</p>
<p>Stored Procedure: sr[InformalTableName]_[FieldName]_[FieldGroup]_[AdditionalDescription]Upd</p></td>
</tr>
<tr class="even">
<td><p>Sub-View for Source Rules</p></td>
<td><p>For Manual Rules only [System won’t generate a namespace for these]:</p>
<p>sr[InformalTableName]_[FieldName]_[AdditionalDescription]_[010]UpdSel or</p>
<p>sr[InformalTableName]_[FieldName]_[AdditionalDescription]_[020]UpdSel</p>
<p>Final registered rule:</p>
<p>sr[InformalTableName]_[FieldName]_[AdditionalDescription]UpdSel</p></td>
</tr>
<tr class="odd">
<td><p>Target Table</p></td>
<td><p>tt[TargetName]</p></td>
</tr>
<tr class="even">
<td><p>Target Source</p></td>
<td><p>st[Target Name]_[Source System ID]</p></td>
</tr>
<tr class="odd">
<td><p>Target Rule</p></td>
<td><p>View: tr[InformalTableName]_[FieldName]UpdSel</p>
<p>Stored Procedure:  tr[InformalTableName]_[FieldName]Upd</p>
<p>If Field Groups are being used:</p>
<p>View: tr[InformalTableName]_[FieldName]_[FieldGroup]UpdSel</p>
<p>Stored Procedure: tr[InformalTableName]_[FieldName]_[FieldGroup]Upd</p>
<p> </p>
<p>If Field Groups are not being used:</p>
<p>For Manual Rules (System won’t generate a namespace for these):</p>
<p>View: tr[InformalTableName]_[FieldName]_[FieldGroup]_[AdditionalDescription]UpdSel</p>
<p>Stored Procedure: tr[InformalTableName]_[FieldName]_[FieldGroup]_[AdditionalDescription]Upd</p></td>
</tr>
<tr class="even">
<td><p>Target Report</p></td>
<td><p>tv[InformalTableName]_[FieldName]_[Description]Sel or</p>
<p>tv[InformalTableName]_[Fieldname]Sel or</p>
<p>tv[InformalTableName]_[Description]Sel</p>
<p> </p>
<p>For Manual Reports the same naming convention should be followed.</p></td>
</tr>
<tr class="odd">
<td><p>Target Export</p></td>
<td><p>tx[InformalTableName]_[Description]Sel</p>
<p>tx[InformalTableName]_[FieldName]Sel or</p>
<p>tx[InformalTableName]_[Description]BDC</p></td>
</tr>
<tr class="even">
<td><p>Import Packages (Created in Assemble)</p></td>
<td><p>#Database#%#Source#%.imp</p></td>
</tr>
<tr class="odd">
<td><p>Export packages (Created in Assemble)</p></td>
<td><p>#Database#%#Source#%.exp</p></td>
</tr>
</tbody>
</table>
