+++
title = 'Index Columns'
solution = 'Platform'
+++

# Index Columns

<div class="use">

Use this page to [Add a Column to an
Index](../Use_Cases/Add%20a%20Column%20to%20an%20Index).

</div>

To access this page:

1.  Select **Admin \> Data Sources** in the *Navigation* pane.
2.  Click the **Index** icon for a data source.
3.  Click the **Columns** icon for a table.

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
<td><p>COLUMN</p></td>
<td><p>Displays the name of the column that is indexed.</p>
<p><strong>NOTE</strong>: An encrypted column cannot be indexed. </p></td>
</tr>
<tr class="odd">
<td><p>DICTIONARY ID</p></td>
<td><p>Displays the name of the dictionary used when searching on this column. Dictionaries contain words and their synonyms that are used to resolve abbreviations or to normalize common industry or company-specific abbreviations. Refer to <a href="../Use_Cases/Create_Dictionaries">Create Dictionaries</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>SEARCHABLE</p></td>
<td><p>If enabled, the column is searchable for indexing. </p>
<p><strong>NOTE</strong>: If a field must be marked as a key field in the DSP®, even though it is not a key field in the underlying table, this check box is disabled.</p></td>
</tr>
<tr class="odd">
<td><p>DUPLICATE DETECTION</p></td>
<td><p>If enabled, the column can be searched during the Duplicate Detection process, used to identify and resolve duplicate data. Refer to Find Duplicates Overview in Common help for more information.</p></td>
</tr>
<tr class="even">
<td><p>KEY</p></td>
<td><p>If enabled, the column is the primary key on the table.</p></td>
</tr>
</tbody>
</table>
