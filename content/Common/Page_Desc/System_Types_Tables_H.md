+++
title = 'System Types Tables H'
solution = 'Platform'
+++

# System Types Tables H

[System Types Tables V](#SystemTypesTablesV)

<div class="use">

Use this page to

  - [Manually Add System
    Tables](../Use_Cases/Manually_Add_System_Tables.htm)
  - [Copy a System Type
    Table](../Use_Cases/Copy_a_System_Type_Table1.htm)

</div>

To access this page:

1.  Select **Common \> System Types** in the *Navigation* pane.
2.  Click the **Tables** icon for the System Type.

<span style="font-weight: bold;">NOTE:</span> Excel Integration has been
enabled on this page. Refer to [Use Excel
Integration](../../Excel_Int/Use_Excel_Integration.htm) for more
information.

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
<td><p>TABLE NAME</p></td>
<td><p>Displays table name within the System Type.</p>
<p><strong>NOTE:</strong> The validation will fail if the table name is not unique.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays brief description of the table.</p></td>
</tr>
<tr class="even">
<td><p>Fields</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="System_Types_Table_Fields_H.htm">System Types Table Fields</a></span> page to add, edit and delete table fields.</p></td>
</tr>
<tr class="odd">
<td><p>Indices</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="System_Types_Table_Indices.htm">System Type Table Indices</a></span> page  to add, edit and delete table indexes.</p></td>
</tr>
<tr class="even">
<td><p>Joins</p></td>
<td><p>Click to open the <em><a href="System_Types_Joins.htm">System Types Joins</a></em> page to add, edit and delete joins for the System Type.</p></td>
</tr>
<tr class="odd">
<td><p>DSP SUPPLIED</p></td>
<td></td>
</tr>
</tbody>
</table>

## <span id="SystemTypesTablesV"></span>System Types Tables V All Tabs

[System Types Tables H](#top)

<div class="use">

Use this page to

  - [Manually Add System
    Tables](../Use_Cases/Manually_Add_System_Tables.htm)
  - [Copy a System Type
    Table](../Use_Cases/Copy_a_System_Type_Table1.htm)

</div>

This page contains the following tabs:

  - [General tab](#General_Tab1)
  - [Copy tab](#Copy_Tab)
  - [Audit Information tab](#Audit_Information_Tab)

## <span id="General_Tab1"></span>General tab

Field

Description

System Type

Displays name of the external system.

Table Name

Displays table name within the System Type.

Description

Displays brief description of the table.

Description Table

Description Table

Displays the name of the table that stores the descriptions for the
values in the value table.

**NOTE**: This field displays in Map in the Description Table field on
the *Vertical* View of the *[Value Mapping
(Config)](../../../Migration/Map/Page_Desc/Value_Mapping_Config_H.htm)*
page).

Description Table Field

Displays the name of the column that stores the descriptions for the
values in the value table.

This field displays in Map in the Description Field field on the
*Vertical* View of the *[Value Mapping
(Config)](../../../Migration/Map/Page_Desc/Value_Mapping_Config_H.htm)*
page).

Description Table Key Field

Displays the key column on the Description table used to uniquely
identify values if the Description table key is different from the Value
table's key column.

This field is used by the T006 table.

**NOTE**: If this field is blank, the Description Table Key uses the
Value Table Key.

Description Table Client Field

Displays the column on the Description Table that stores the Client or
Tenant of the data. Used with SAP only.

Description Table Language Field

Displays the column on the Description Table that stores the language
identifier column. Used with SAP only.

Lookup Table

<span id="Lookup Table Type" class="popUpLink">Lookup Table Type</span>

Displays an option indicating whether fields in the lookup table should
be value mapped.

Lookup Table Field 1

Displays the key in the lookup table.

Lookup Table Field 2

Displays the second key in a lookup table with a multipart key.

Lookup Table Field 3

Displays the third key in a lookup table with a multipart key.

Lookup Table Field 4

Displays the fourth key in a lookup table with a multipart key.

Lookup Table Field 5

Displays the fifth key in a lookup table with a multipart key.

Lookup Table Field Value

Displays the column on the lookup table that stores the Client or Tenant
of the data. Used with SAP only.

Lookup Table Client Field

Displays the column on the lookup table that stores the language
identifier column. Used with SAP only.

Lookup Table Language Field

Displays the field used for the value in the update row rule when
multiple keys are entered.

Lookup Table Where Clause

Displays the where clause used to filter values in the lookup table
column to restrict the values used in the lookup table.

## <span id="Copy_Tab"></span>Copy tab

<div class="use">

Use this tab to [Copy a System Type
Table](../Use_Cases/Copy_a_System_Type_Table1.htm).

</div>

Field

Description

Copy Table

Copy to Table Name

Displays a blank field that the user completes when copying a table.
Once the table is copied, the field is blank again.

Copy To Table

Click to copy the current table to create a new table listed in the Copy
To Table Name field. Any fields and lookup table fields are also copied
to the new table. If the new table name already exists, any fields or
lookup table fields that do not exist for the table are added. No tables
are updated or deleted.

## <span id="Audit_Information_Tab"></span>Audit Information tab

Field

Description

Tracking

Added By

Displays user ID of individual who added the system table. This field
can also display the following:

  - **FetchTable** – when the fetch table process adds the System Type.
    This process reads the Collect source to download a list of tables
    from the client source systems.
  - **BulkImport** – when the bulk import process adds the System Type.
    “Bulk Import” is a generic term used to insert large amounts of
    data into SQL server databases. In this scenario, a bulk import is
    performed to load System Types into the database.

Added On

Displays date and time when user ID added the system table.

Changed By

Displays user ID of individual who updated the system table.

Changed On

Displays date and time when user ID updated the system table.
