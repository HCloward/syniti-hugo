+++
title = 'Create all tt Tables and tx Views for the Integrate Process'
solution = 'Data Quality'
+++

# Create all tt Tables and tx Views for the Integrate Process

Before performing this task, create a looped template and process in
Integrate. Refer to [Configure Process Template Loops for a BDC Script
Template with Looping
Enabled](../../../Platform/Integrate/Use_Cases/ConfigureProcTempLoopsBDCLoopEn.htm)
or [Configure Process Template Loops for a GUI Script Template with
Looping
Enabled](../../../Platform/Integrate/Use_Cases/ConfigureProcTemplLoopsGUILoopgEn.htm)
in Integrate for more information.

Create the **tt** tables and **tx** views for the each loop -- header
and detail data -- manually or by using the Auto Generate functionality
in Integrate. Refer to [Generate Database Objects
Automatically](../../../Platform/Integrate/Use_Cases/Generate_Database_Objects_Automatically.htm)
for more information.

Tables and views may be created in cMass\_Data or any database that has
a supporting component and data source registered in the DSP®.

If using auto-generated tables, add these columns to each **tt** table.
If manually generating the tables, include these columns:

<span style="font-weight: bold;">NOTE</span>: ID column must be set as
the PrimaryKey of the tt Table.

 

<table>
<tbody>
<tr class="odd">
<td><p>Column Name</p></td>
<td><p>Data Type</p></td>
<td><p>Value</p></td>
</tr>
<tr class="even">
<td><p>RequestID</p>
<p><strong>NOTE</strong>: Place this column underneath the ID and ParentID columns.</p></td>
<td><p>int</p></td>
<td><p>NULL</p></td>
</tr>
<tr class="odd">
<td><p>PostError</p></td>
<td><p>int</p></td>
<td><p>NULL DEFAULT (2)</p></td>
</tr>
<tr class="even">
<td><p>PostMessage</p></td>
<td><p>nvarchar (max)</p></td>
<td><p>NULL DEFAULT ''</p></td>
</tr>
<tr class="odd">
<td><p>boaStatus</p></td>
<td><p>int</p></td>
<td><p>NULL</p></td>
</tr>
<tr class="even">
<td><p>ValidationErrorMessage</p></td>
<td><p>nvarchar (max)</p></td>
<td><p>NULL</p></td>
</tr>
<tr class="odd">
<td><p>Severity</p></td>
<td><p>int</p></td>
<td><p>NULL</p></td>
</tr>
<tr class="even">
<td><p>Reject</p></td>
<td><p>bit</p></td>
<td><p>NULL DEFAULT (0)</p></td>
</tr>
<tr class="odd">
<td><p>RejectReason</p></td>
<td><p>nvarchar (max)</p></td>
<td><p>NULL</p></td>
</tr>
<tr class="even">
<td><p>RejectedBy</p></td>
<td><p>nvarchar (50)</p></td>
<td><p>NULL</p></td>
</tr>
<tr class="odd">
<td><p>LockReject</p></td>
<td><p>bit</p></td>
<td><p>NULL</p></td>
</tr>
</tbody>
</table>

 

Continue with [Create rt Tables from the tt
Tables](Create_rt_Tables_from_the_tt_Tables.htm).
