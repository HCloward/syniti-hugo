+++
title = 'Connection Types H'
solution = 'Platform'
+++

# Connection Types H

[Connection Types V](#Connection_Types_V)

<div class="use">

Use this page to [Set Up Connection
Types](../Config/Set_up_Connection_Types).

</div>

To access this page, select <span style="font-weight: bold;">Collect \>
Administrative \> Connection Types</span> in
<span style="font-style: italic;">Navigation</span>
pane.

|                        |                                                                                                                                                                                      |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field                  | Description                                                                                                                                                                          |
| TARGET CONNECTION TYPE | Displays the database connection type for the target.                                                                                                                                |
| OLE PROVIDER           | Displays name of OLE settings.                                                                                                                                                       |
| ODBC DRIVER            | Displays name of driver used in the Windows ODBC setup for the DSN.                                                                                                                  |
| Sources                | Click to open the <span style="font-style: italic;">[Source Connection Types](Source_Connection_Types_H)</span> page to add, edit and delete sources connections for the target. |

## <span id="Connection_Types_V"></span>Connection Types V

[Connection Types H](Connection_Types_H)

<div class="use">

Use this page to [Set Up Connection
Types](../Config/Set_up_Connection_Types).

</div>

|                           |                                                                                                                                                                                                                                                                                                                                                                                           |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                     | Description                                                                                                                                                                                                                                                                                                                                                                               |
| Target Connection Type    | Displays the database connection type for the target.                                                                                                                                                                                                                                                                                                                                     |
| Download Table SQL        | Displays the SQL command used to download all tables in a database and inserts them into a group that has the same name as the Connection. If the group does not exist, the process creates the group and inserts all the tables into the group from the database.<span class="appleconvertedspace" style="font-family: Verdana, sans-serif;color: #000000;background: #ffffff;"> </span> |
| Createtable SQL           | Displays the SQL called during the Fetch Table process. A list of tables that is available to download from source is downloaded.                                                                                                                                                                                                                                                         |
| Create Primary Key SQL    | Displays the SQL called during the Build Package process. Only used for non-SAP systems. Checks to see if the table built from the SQL has any primary keys attached. If blank, a new table in SQL will not have primary keys.                                                                                                                                                            |
| Create Index SQL          | Displays the SQL used to create index.                                                                                                                                                                                                                                                                                                                                                    |
| OLE Provider              | Displays name of OLE settings.                                                                                                                                                                                                                                                                                                                                                            |
| Connection String Example | Displays an example of a connection string for reference.                                                                                                                                                                                                                                                                                                                                 |
| Left Column Delimiter     | Displays the character that wraps around the left of columns and table names.                                                                                                                                                                                                                                                                                                             |
| Right Column Delimiter    | Displays the character that wraps around the right of columns and table names.                                                                                                                                                                                                                                                                                                            |
