+++
title = 'Data Source Table Columns H'
solution = 'Platform'
+++

# Data Source Table Columns H

[Data Source Table Columns V](#Data_Source_Table1)

<div class="use">

Use this page to [Modify Configuration of Data Source Table
Columns](../Use_Cases/Modify_Configuration_of_Data_Source_Table_Columns.htm).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">Collect \> Targets</span> in
    the Navigation pane.
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
8.  Click <span style="font-weight: bold;">Column Count</span> for a
    data source table.

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
<td><p>Displays the column converted to the defined data type and loaded into the target table.</p></td>
</tr>
<tr class="odd">
<td><p>FROM DATA TYPE</p></td>
<td><p>Displays data type of field in the source.</p></td>
</tr>
<tr class="even">
<td><p>FROM DATA LENGTH</p></td>
<td><p>Displays data length of field in the source.</p></td>
</tr>
<tr class="odd">
<td><p>FROM DATA SCALE</p></td>
<td><p>Displays data scale of field (number of digits after decimal point) in the source.</p></td>
</tr>
<tr class="even">
<td><p>TABLE CREATE DATA TYPE</p></td>
<td><p>Displays definition used in SQL Server to create tables in the target.</p></td>
</tr>
<tr class="odd">
<td><p>COLUMN OVERRIDE</p></td>
<td><p>Displays the source system SQL function or command to download data from the source.</p>
<p><strong>NOTE:</strong> The Column Override field allows for source system function commands to be overridden when data is loaded into the target SQL server tables, for example, TO_CHAR(ORDER_TIMESTAMP,’YYYYMMDD’) as Order_Timestamp.</p></td>
</tr>
<tr class="even">
<td><p>COLUMN ORDER</p></td>
<td><p>Displays the exact order of columns within the table. This value can get large because it’s a unique value for all tables and columns.</p></td>
</tr>
</tbody>
</table>

## <span id="Data_Source_Table1"></span>Data Source Table Columns V

[Data Source Table Columns H](Data_Source_Table_Columns_H.htm)

<div class="use">

Use this page to [Modify Configuration of Data Source Table
Columns](../Use_Cases/Modify_Configuration_of_Data_Source_Table_Columns.htm).

</div>

|                        |                                                                                                                                    |
| ---------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| Field                  | Description                                                                                                                        |
| Column                 | Displays the column converted to the defined data type and loaded into the target table.                                           |
| From Data Type         | Displays data type of field in the source.                                                                                         |
| From Data Length       | Displays data length of field in the source.                                                                                       |
| From Data Precision    | Displays data precision of field (total number of digits) in the source.                                                           |
| From Data Scale        | Displays data scale of field (number of digits after decimal point) in the source.                                                 |
| From Nullable          | Displays nullable flag of field in the source.                                                                                     |
| Table Create Data Type | Displays data type to create tables in the database.                                                                               |
| To Data Type           | Displays new data type of field in the target.                                                                                     |
| To Data Length         | Displays new data length of field in the target.                                                                                   |
| To Data Precision      | Displays new data precision of field (total number of digits) in the target.                                                       |
| To Data Scale          | Displays new data scale of field (number of digits after decimal point) in the target.                                             |
| To Nullable            | Displays new nullable flag of field in the target.                                                                                 |
| Column Override        | Displays the source system SQL function or command to download data from the source.                                               |
| Column Order           | Displays exact order of columns within the table. This value can get large because it’s a unique value for all tables and columns. |
