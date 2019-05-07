+++
title = 'Create all tt Tables and Views for the BAPI Process'
solution = 'Data Quality'
+++

# Create all tt Tables and Views for the BAPI Process

Before performing these steps, [Post Data Using A
BAPI](../../../Platform/Integrate/Use_Cases/Post_Data_Using_a_BAPI.htm).

Manually build tables (a main table and an upload table) and views in
any database that has a supporting component and data source that is
registered in the DSP®.

Using the auto-generated BAPI tables that exist in Integrate, script
each BAPI table as a new table beginning with **tt**. In addition to the
existing columns, add the following columns to each **tt** table:

<span style="font-weight: bold;">NOTE</span>: The ID column must be set
as the PrimaryKey of the tt Table.

<table>
<tbody>
<tr class="odd">
<td><p>Column Name</p></td>
<td><p>Data Type</p></td>
<td><p>Value</p></td>
</tr>
<tr class="even">
<td><p>RequestID</p>
<p><strong>NOTE</strong>: Place this column at the top underneath ID.</p></td>
<td><p>int</p></td>
<td><p>NULL, &lt;-</p></td>
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

Continue with [Create rt Tables From the tt Tables and Create Views for
the BAPI Process](CreatertTblsttTableCreateVwsBAPI.htm).
