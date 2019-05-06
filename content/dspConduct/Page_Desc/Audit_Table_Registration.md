# Audit Table Registration

<div class="use">

Use this page to [Register Tables and Columns to be
Audited](../Use_Cases/Review_Request_Changes.htm#Register_Tables_and_Columns_to_be_Audited).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Vertical View</span> for a
    category.
3.  Click the <span style="font-weight: bold;">Rules and Actions</span>
    tab.
4.  Click the <span style="font-weight: bold;">Table Registration</span>
    icon.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Load Audit Data</p></td>
<td><p>Click to copy new audit data associated with the current category to the dspConduct™ Review Role staging tables immediately.</p>
<p><strong>NOTE:</strong> Copying audit data immediately is not required. Audit data is automatically copied to the staging tables when table or column registrations are updated.</p></td>
</tr>
<tr class="odd">
<td><p>TABLE NAME</p></td>
<td><p>Displays the name of the table that has auditing enabled.</p></td>
</tr>
<tr class="even">
<td><p>LAST IMPORTED ON</p></td>
<td><p>Displays the date and time the table was last imported.</p></td>
</tr>
<tr class="odd">
<td><p>LAST AUDIT ID</p></td>
<td><p>Displays the audit ID assigned to the last audit conducted for the table.</p></td>
</tr>
<tr class="even">
<td><p>ENABLED</p></td>
<td><p>If enabled, auditing is turned on for the table. If disabled, the table data is not audited.</p>
<p><strong>NOTE:</strong> If auditing is disabled for a table, it is also disabled for all columns in the table, and no columns display on the <a href="Audit_Table_Column_Registration.htm">Audit Table Column Registration</a> page. Additionally, changes associated with the table do not display to the Review role when reviewing changes on the Review Role Audit Details page.</p></td>
</tr>
<tr class="odd">
<td><p>Columns</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Audit_Table_Registration.htm">Audit Table Column Registration</a></span> page to include or exclude columns from auditing.</p></td>
</tr>
</tbody>
</table>
