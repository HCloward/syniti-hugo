# Database Import

<div class="use">

Use this page to [Import Target Design from a
Database](../Use_Cases/Import_from_a_Database.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Select <span style="font-weight: bold;">Design </span>in the Context
    bar.
3.  Click <span style="font-weight: bold;">Target Import</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
4.  Click the <span style="font-weight: bold;">Database
    Import</span>icon for an Object.
5.  Click the **Import** icon for the DATA SOURCE.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Mark for Import</p></td>
<td><p>Click to enable the IMPORT check box for multiple selected tables to include the tables in the import.</p></td>
</tr>
<tr class="odd">
<td><p>Clear Import Flag</p></td>
<td><p>Click to disable the IMPORT check box for multiple selected tables to exclude the tables from import.</p></td>
</tr>
<tr class="even">
<td><p>Execute Import</p></td>
<td><p>Click to perform the import for those tables with the IMPORT check box enabled. The import process brings the tables and fields into the Target for the selected Object.</p>
<p>Once imported, the tables become a Target of the Object, and are accessible on the <span style="font-style: italic;"><a href="Targets_H_Design.htm">Targets</a></span> page.</p>
<p>During the import, new records are added to the tables, fields, and look up tables. If the records have been imported into the Target previously, updates are applied to existing tables, fields and lookup tables.</p></td>
</tr>
<tr class="odd">
<td><p>OBJECT ID</p></td>
<td><p>Displays the Object that will contain the Target table once it is imported. contains the Target.</p>
<p>Objects are added in Console. Refer to <a href="../../Console/Use_Cases/Add_Elements_Separately.htm#Add3">Add an Object</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>TABLENAME</p></td>
<td><p>Displays the name of the table in the database that will be imported into the Target if the IMPORT check box is enabled.</p>
<p>The TABLENAME displays on the <span style="font-style: italic;">Targets</span> page (Design &gt; Targets) once imported.</p></td>
</tr>
<tr class="odd">
<td><p>IMPORT</p></td>
<td><p>If checked, the table will be imported into the Target when the user clicks the Execute Import icon. If unchecked, the table is excluded from import.</p></td>
</tr>
</tbody>
</table>
