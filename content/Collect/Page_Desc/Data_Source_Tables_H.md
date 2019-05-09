+++
title = 'Data Source Tables H'
solution = 'Platform'
+++

# Data Source Tables H

[Data Source Tables V](#Data_Source_Tables_V)

<div class="use">

Use this page to [Modify Configuration of Data Source
Tables](../Use_Cases/Modify_Configuration_of_Data_Source_Tables).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">Collect \> Targets</span> in
    the <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Sources</span> for a target.
3.  Click <span style="font-weight: bold;">Schedule Groups</span> for a
    source.
4.  Click <span style="font-weight: bold;">Tables</span> for a schedule
    group.
5.  Click <span style="font-weight: bold;">Vertical View</span> for a
    table.
6.  Click <span style="font-weight: bold;">General Information</span>
    tab.
7.  Click <span style="font-weight: bold;">View
Design</span>.

|              |                                                                                                                                                                                                                                                           |
| ------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field        | Description                                                                                                                                                                                                                                               |
| TABLE        | Displays table in source.                                                                                                                                                                                                                                 |
| TARGET       | Displays database where tables are refreshed with source data.                                                                                                                                                                                            |
| SOURCE       | Displays database where data is refreshed from and stored in the target.                                                                                                                                                                                  |
| PACKAGE NAME | Displays name of package that refreshes target table with source data.                                                                                                                                                                                    |
| BUILT COUNT  | Displays the number of times the package has been built.                                                                                                                                                                                                  |
| Column Count | Displays number of columns in source table. Click link to open the <span style="font-style: italic;">Data Source Table Columns</span><span>page to add, edit and delete</span> columns within source table.                                               |
| SQL Command  | Click to open the <span style="font-style: italic;">[<span style="font-style: italic;">Data Source Table Create Download SQL</span>](Data_Source_Table_Create_Download_SQL_H)</span><span>page to edit and delete</span> SQL commands in the package. |

## <span id="Data_Source_Tables_V"></span>Data Source Tables V

[Data Source Tables H](Data_Source_Tables_H)

<div class="use">

Use this page to [Modify Configuration of Data Source
Tables](../Use_Cases/Modify_Configuration_of_Data_Source_Tables).

</div>

|                 |                                                                                                                                                               |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field           | Description                                                                                                                                                   |
| Target          | Displays database where tables are refreshed with source data.                                                                                                |
| Source          | Displays database where data is refreshed from and stored in the target<span style="font-family: Calibri, sans-serif;">.</span>                               |
| Table           | Displays table in source.                                                                                                                                     |
| Table Rename    | Displays table name of renamed table in target. New table name must contain \[TableName\]. At run time, \[TableName\] is replaced with processing table name. |
| Package Name    | Displays name of package that refreshes target table with source data.                                                                                        |
| Target Time Out | Displays time out period, in seconds, for the target. Default value is **180** (3 minutes).                                                                   |
| Source Time Out | Displays time out period, in seconds, for the source. Default value is **300** (5 minutes).                                                                   |
| Built Count     | Displays the number of times the package has been built.                                                                                                      |
