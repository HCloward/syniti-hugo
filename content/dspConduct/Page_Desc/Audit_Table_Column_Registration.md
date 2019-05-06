# Audit Table Column Registration

<div class="use">

Use this page to [Register Tables and Columns to be
Audited](../Use_Cases/Review_Request_Changes.htm#Register_Tables_and_Columns_to_be_Audited).

</div>

To access this page:

1.  Click **dspConduct \> Design** in the *Navigation* pane.
2.  Click **Vertical View** for a category.
3.  Click the **Rules and Actions** tab.
4.  Click the **Table Registration** icon.
5.  Click the **Columns** icon for a table.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>COLUMN NAME</p></td>
<td><p>Displays the technical field name of the column to be audited.</p>
<p><strong>NOTE:</strong> If the table to which the column belongs is not enabled for auditing (i.e., the ENABLED check box is not selected for the table on the Audit Table Registration page) no data displays on this page.</p></td>
</tr>
<tr class="odd">
<td><p>ENABLED</p></td>
<td><p>If enabled, data in that column is audited. If disabled, data is not audited.</p></td>
</tr>
<tr class="even">
<td><p>DISPLAY COLUMN NAME</p></td>
<td><p>Displays the column description.</p></td>
</tr>
<tr class="odd">
<td><p>PRIMARY KEY</p></td>
<td><p>If checked, the column is the key field on the table, or is part of the multi-part key. This column displays by default in the Key to Record field on the <em><a href="Review_Role_Audit_Details_H.htm">Review Role Audit Details</a></em> page when the check box is checked.</p>
<p>If unchecked, the Key to Record field does not display on the Review Role Audit Detail page.</p></td>
</tr>
<tr class="even">
<td><p>INCLUDE IN RECORD KEY</p></td>
<td><p>If enabled, the column name is included, along with the key field(s), in the Key to Record field on the <em>Review Role Audit Details</em> page. If disabled the column name does not display.</p>
<p><strong>NOTE:</strong> Key fields are not affected by this setting, with the exception of the RequestID. Key fields display in the Key to Record field, even if this check box is disabled. However, the display of the RequestID column can be controlled using this option. For example, the user disables this option for the key fields DATE_FROM and RequestID. In the Key to Record field, the DATE_FROM field still displays. The RequestID field does not.</p></td>
</tr>
</tbody>
</table>
