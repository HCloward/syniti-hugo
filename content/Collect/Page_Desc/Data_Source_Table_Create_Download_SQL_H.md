+++
title = ''
solution = 'Platform'
+++

# <span id="top"></span>Data Source Table Create Download SQL H

[Data Source Table Create Download SQL V](#Data_Source_Table_Create1)

<div class="use">

Use this page to [View Configuration of Data Source Table SQL
Commands](../Use_Cases/View_Configuration_of_Data_Source_Table_SQL_Commands.htm).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">Collect \> Targets</span> on
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Sources</span> for a target.
3.  Click <span style="font-weight: bold;">Schedule Groups</span> for a
    source.
4.  Click <span style="font-weight: bold;">Tables</span> for a schedule
    group.
5.  Click <span style="font-weight: bold;">Vertical View</span> for a
    table.
6.  Click <span style="font-weight: bold;">General Information</span>
    tab.
7.  Click <span style="font-weight: bold;">View Design</span>.
8.  Click<span style="font-weight: bold;"> SQL Command</span> for a data
    source table.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>TABLE</p></td>
<td><p>Displays name of table refreshed from source to target.</p></td>
</tr>
<tr class="odd">
<td><p>SQL COMMAND</p></td>
<td><p>Displays the SQL commands that are run when the table is created on a build or download process.</p></td>
</tr>
<tr class="even">
<td><p>RECORD TYPE</p></td>
<td><p>Displays the type of record (as in, the SQL command).</p>
<p>Values are:</p>
<ul>
<li><strong>Clustered Index</strong> - Creates a cluster index on the target table</li>
<li><strong>Create Table</strong> - Creates the table in the target database</li>
<li><strong>Indexes</strong> - Creates an index on the target table</li>
<li><strong>Primary Key</strong> - Creates the primary key on the target table</li>
<li><strong>Select Table</strong> - Selects * from the source table</li>
</ul></td>
</tr>
</tbody>
</table>

## <span id="Data_Source_Table_Create1"></span>Data Source Table Create Download SQL V

[Data Source Table Create Download SQL H](#top)

<div class="use">

Use this page to [View Configuration of Data Source Table SQL
Commands](../Use_Cases/View_Configuration_of_Data_Source_Table_SQL_Commands.htm).

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
<td><p>Target</p></td>
<td><p>Displays the database where tables are refreshed with source data.</p></td>
</tr>
<tr class="odd">
<td><p>Source</p></td>
<td><p>Displays the database where data is refreshed from and stored in the target.</p></td>
</tr>
<tr class="even">
<td><p>Table</p></td>
<td><p>Displays name of the table refreshed from source to target.</p></td>
</tr>
<tr class="odd">
<td><p>Record Type</p></td>
<td><p>Displays the type of record (i.e., the SQL command).</p>
<p>Values are:</p>
<ul>
<li><strong>Clustered Index</strong> - Creates a cluster index on the target table</li>
<li><strong>Create Table</strong> - Creates the table in the target database</li>
<li><strong>Indexes</strong> - Creates an index on the target table</li>
<li><strong>Primary Key</strong> - Creates the primary key on the target table</li>
<li><strong>Select Table</strong> - Selects * from the source table</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Record Order</p></td>
<td><p>Displays logical sort order of records in the table.</p></td>
</tr>
<tr class="odd">
<td><p>SQL Command</p></td>
<td><p>Displays the SQL commands that are run when the table is created on a build or download process.</p></td>
</tr>
</tbody>
</table>
