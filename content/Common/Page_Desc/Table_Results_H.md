+++
title = 'Table (Results) H'
solution = 'Platform'
+++

# Table (Results) H

### [Table (Results) V](Table_Results_H#Table__Results__V)

<div class="use">

Use this page to

  - [Activate and Deactivate
    Tables](../Use_Cases/Activate_and_Deactivate_Tables)
  - [Profile Individual
    Tables](../Use_Cases/Profile_Data_Sources#Profile_Individual_Tables)
  - [View Table
    Results](../../../Migration/Construct/Use_Cases/View_Table_Results)
  - [Reset for a Table](../Use_Cases/Reset_Profiling)

</div>

This page can be accessed in two ways.

To access this page to view a list of all tables that are profiled::

1.  Select <span style="font-weight: bold;">Common \> Analyze</span> in
    the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Profile icon</span> for a
    data source.
3.  Click the <span style="font-weight: bold;">Tables</span> icon.

To access this page to view details about a specific table:

1.  Select <span style="font-weight: bold;">Common \> Analyze</span> in
    the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Profile</span> icon for a
    data source.
3.  Click the <span style="font-weight: bold;">Tables</span> icon.
4.  Click the <span style="font-weight: bold;">View Data</span> icon for
    a
table.

|                       |                                                                                                                                                            |
| --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                 | Description                                                                                                                                                |
| Activate All Tables   | Click to activate all tables in the data source (i.e., make them available for profiling). This icon is disabled if all tables are active.                 |
| Inactivate All Tables | Click to deactivate all tables in the data source (i.e., make them unavailable for profiling). This icon is disabled if all tables are inactive.           |
| TABLE                 | Displays the table within the profiled data source.                                                                                                        |
| ACTIVE                | If enabled, the table is profiled for the data source.                                                                                                     |
| LAST UPDATED ON       | Displays the date and time when the table was most recently profiled.                                                                                      |
| RECORD COUNT          | Displays the number of records in the table.                                                                                                               |
| View Data             | Click to view details of the table data.                                                                                                                   |
| Fields                | Click to open the <span style="font-style: italic;">[Table Field (Results)](Table_Field_Results_H)</span> page to  view fields for the profiled table. |
| Execute               | Click to re-profile the data in the tables and rebuild the result set.                                                                                     |
| Reset                 | Click to reset a running profile in the event an error occurs.                                                                                             |

## <span id="Table__Results__V"></span>Table (Results) V

### [Table (Results) H](Table_Results_H)

Field

Description

Table Properties

Table

Displays the table within the profiled data source

Schema Owner

Displays the owner of the table. Default is **dbo**.

Profile Information

Record Count

Displays the number of records in the table.

Total Column Count

Displays the number of columns in the table.

Process Column Count

Displays the number of columns that were profiled for the table.

Last Updated On

Displays the date when the profiling was last run.

Interesting

If enabled, 10% of the table fields are blank.

Process Information

Column Process Started On

Displays the date and time when table profiling started.

Column Process Completed On

Displays the date and time when table profiling completed.

Column Scan Duration

Displays the total time the table profiling took to run.

Unique Process Started On

Displays the start time of the unique process, which finds the
occurrence count of the first 1000 unique values in the table column.

Unique Process Completed On

Displays the end time of the unique process, which finds the occurrence
count of the first 1000 unique values in the table column.

Unique Scan Duration

Displays the time in seconds the unique process ran.

Reset

Click to reset a running profile in the event an error occurs.
