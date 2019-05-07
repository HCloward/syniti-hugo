+++
title = 'Table (Indices) H'
solution = 'Platform'
+++

# Table (Indices) H

[Table (Indices) V](#Table_Indices_V)

<div class="use">

Use this page to [Create Indices for
Tables](../Use_Cases/Add_Rules_and_Indices_to_Tables.htm#Create_Indices_for_Tables).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Tables</span> on the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Indices</span> icon for a
    table.

|                 |                                                                                                                                                                                                           |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field           | Description                                                                                                                                                                                               |
| Build Index     | Click to schedule the rebuild process for all indices in the Target Source table index. Only keys stored in the table are rebuilt.                                                                        |
| INDEX ID        | Displays name of index.                                                                                                                                                                                   |
| UNIQUE INDEX    | If enabled, a unique index is built. The primary key can’t also be enabled. If Unique Index and Primary Key are both disabled, a non-unique index is built. Default value is Disabled.                    |
| PRIMARY KEY     | If enabled, index is built as a primary key for the table. Unique Index can’t also be enabled. If Unique Index and Primary Key are both disabled, a non-unique index is built. Default value is Disabled. |
| CLUSTERED INDEX | If enabled, index is marked as <span style="font-style: italic;">clustered</span>.  Default value is Disabled.                                                                                            |
| SOURCE DOWNLOAD | If enabled, index settings were downloaded to the table. Otherwise, the index was supplied from group tables. This setting cannot be updated from within Collect.                                         |
| Columns         | Click to open the <span style="font-style: italic;">[Target Source Table Index Column](Target_Source_Table_Index_Columns.htm)</span> page to add, edit and delete columns for table index.                |

## <span id="Table_Indices_V"></span>Table (Indices) V

[Table (Indices) H](Table_Indices_H.htm)

<div class="use">

Use this page to [Create Indices for
Tables](../Use_Cases/Add_Rules_and_Indices_to_Tables.htm#Create_Indices_for_Tables).

</div>

|                   |                                                                                                                                                                                                               |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field             | Description                                                                                                                                                                                                   |
| Build Index       | Click to schedule the rebuild process for all indices in the Target Source table index. Only keys stored in the table are rebuilt.                                                                            |
| Index ID          | Displays name of the index.                                                                                                                                                                                   |
| Unique Index      | If enabled, a unique index is built. The primary key can’t also be enabled. If Unique Index and Primary Key are both disabled, a non-unique index is built. Default value is Disabled.                        |
| Primary Key       | If enabled, the index is built as a primary key for the table. Unique Index can’t also be enabled. If Unique Index and Primary Key are both disabled, a non-unique index is built. Default value is Disabled. |
| Source Download   | If enabled, index settings were downloaded to the table. Otherwise, the index was supplied from group tables. This setting cannot be updated from within Collect.                                             |
| Index SQL Command | Displays command that is run to create the index. Value is auto-generated.                                                                                                                                    |
| Columns           | Click to open the <span style="font-style: italic;">[Target Source Table Index Column](Target_Source_Table_Index_Columns.htm)</span> page to add, edit and delete columns for table index.                    |
