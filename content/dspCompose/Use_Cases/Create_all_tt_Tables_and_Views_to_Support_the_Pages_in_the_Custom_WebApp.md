+++
title = 'Create all tt Tables and Views to Support the Pages in the Custom WebApp'
solution = 'Data Quality'
+++

# Create all tt Tables and Views to Support the Pages in the Custom WebApp

Manually build tables and views in any database that has a supporting
component and data source that is registered in the DSP®. Find an
automatically created tt Data Entry table in cMass\_Data and use as an
example.

If the template has been recorded and will support request posting, the
tt table should include any columns from the recording. In addition to
the recorded columns, the following columns must exist in the tt table.

**NOTE:** The ID column must be set as the PrimaryKey of the tt Table.

<table>
<tbody>
<tr class="odd">
<td><p>Column Name</p></td>
<td><p>Data Type</p></td>
<td><p>Value</p></td>
</tr>
<tr class="even">
<td><p>ID</p></td>
<td><p>int</p></td>
<td><p>IDENTITY(1,1) NOT NULL</p></td>
</tr>
<tr class="odd">
<td><p>RequestID</p>
<p>NOTE: Place this column at the top underneath ID.</p></td>
<td><p>int</p></td>
<td><p>NULL, &lt;-</p></td>
</tr>
<tr class="even">
<td><p>PostError</p></td>
<td><p>int</p></td>
<td><p>NULL DEFAULT (2)</p></td>
</tr>
<tr class="odd">
<td><p>PostMessage</p></td>
<td><p>nvarchar (max)</p></td>
<td><p>NULL DEFAULT ''</p></td>
</tr>
<tr class="even">
<td><p>boaStatus</p></td>
<td><p>int</p></td>
<td><p>NULL</p></td>
</tr>
<tr class="odd">
<td><p>ValidationErrorMessage</p></td>
<td><p>nvarchar (max)</p></td>
<td><p>NULL</p></td>
</tr>
<tr class="even">
<td><p>Severity</p></td>
<td><p>int</p></td>
<td><p>NULL</p></td>
</tr>
<tr class="odd">
<td><p>Reject</p></td>
<td><p>bit</p></td>
<td><p>NULL DEFAULT (0)</p></td>
</tr>
<tr class="even">
<td><p>RejectReason</p></td>
<td><p>nvarchar (max)</p></td>
<td><p>NULL</p></td>
</tr>
<tr class="odd">
<td><p>RejectedBy</p></td>
<td><p>nvarchar (50)</p></td>
<td><p>NULL</p></td>
</tr>
<tr class="even">
<td><p>LockReject</p></td>
<td><p>bit</p></td>
<td><p>NULL</p></td>
</tr>
</tbody>
</table>
