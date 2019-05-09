+++
title = 'Task Final Finish Where Clause'
solution = 'Master Data Management'
+++

# Task Final Finish Where Clause

Use this page to [Create a Final Finish Where Clause for a CranPort
Package](../Use_Cases/Create_a_Final_Finish_Where_Clause_for_a_CranPort_Package).

<div class="use">

To access this page:

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the *Navigation* pane.
2.  Click the **Tasks** icon for a category.
3.  Click the **Final Finish Tables** icon for a main parent task.
4.  Click **Vertical View** for a table.
5.  Click the **Where Clause Builder** icon.

</div>

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
<td><p>COLUMN NAME</p></td>
<td><p>Displays name of column, usually the key, being filtered on when the table is downloaded from the source database during the Finish process. The column name contains the values to use for the Where clause.</p></td>
</tr>
<tr class="odd">
<td><p>DATA SOURCE ID</p></td>
<td><p>Displays name of the database that contains the table or view where the Mapped Value is located.</p></td>
</tr>
<tr class="even">
<td><p>TABLE VIEW NAME</p></td>
<td><p>Displays name of the table or view that contains the Mapped Value.</p>
<p>This table or view must already exist in the data source.</p></td>
</tr>
<tr class="odd">
<td><p>MAPPED VALUE</p></td>
<td><p>Displays mapped value column from the table or view name. When the Finish process runs, all values are selected from the mapped value binding on RequestID, and an IN statement is formed for selection from the source to the target database.</p></td>
</tr>
<tr class="even">
<td><p>BEGINNING QUALIFIER</p></td>
<td><p>Displays character placed around the values downloaded during the finish process; default value is a single quote.</p></td>
</tr>
<tr class="odd">
<td><p>ENDING QUALIFIER</p></td>
<td><p>Displays character placed around the values downloaded during the finish process; default value is a single quote.</p></td>
</tr>
<tr class="even">
<td><p>SEPARATOR</p></td>
<td><p>Displays character used for data values downloaded during the finish process; default value is a comma.</p></td>
</tr>
<tr class="odd">
<td><p>WHERE STATEMENT</p></td>
<td><p>Displays format of the where clause; default value is #ColumnName# IN (#Data#). #ColumnName# is the name of the column and #Data# is the list of values separated by the character in the Separator field.</p></td>
</tr>
</tbody>
</table>
