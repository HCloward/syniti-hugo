+++
title = 'System Types Table Lookup'
solution = 'Platform'
+++

# System Types Table Lookup

<div class="use" data-xmlns="">

Use this page to [Add a Lookup Table
Manually](../Use_Cases/Add_a%20Lookup%20Table%20Manually.).

</div>

To access this page:

1.  Select **Common \> System Types** in the *Navigation* pane.
2.  Click the **Tables** icon for a System Type.
3.  Click the **Fields** icon for a Table Name.
4.  Click a lookup table name in the **LOOKUP TABLE** column.

**NOTE:** Excel Integration has been enabled on this page. Refer to [Use
Excel Integration](../../Excel_Int/Use_Excel_Integration) for more
information.

Field

Description

System Type

Displays the name of the external system.

Table Name

Displays table name within the System Type.

Description

Displays brief description of the table.

Description Table

Description Table

Displays the name of the table that stores the descriptions for the
values in the value table.

Description Table Field ID

Displays the name of the column that stores the descriptions for the
values in the value table.

Description Table Key Field

Displays the key column on the Description table used to uniquely
identify values if the Description table key is different from the Value
table's key column.

This field is used by the T006 table.

**NOTE:** If this field is blank, the Description Table Key uses the
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

Lookup Table Field

Displays the key in the lookup table

Lookup Table Field 2

Displays the second key in a lookup table with a multipart key.

Lookup Table Field 3

Displays the third key in a lookup table with a multipart key.

Lookup Table Field 4

Displays the fourth key in a lookup table with a multipart key.

Lookup Table Field 5

Displays the fifth key in a lookup table with a multipart key.

Lookup Table Client Field

Displays the column on the lookup table that stores the Client or Tenant
of the data. Used with SAP only.

Lookup Table Language Field

Displays the column on the lookup table that stores the language
identifier column. Used with SAP only.

Multi Value Field Lookup Table Value Field

Displays the column containing the value to use if more than one value
table column is set for the value table (for example, there is data in
the Check Table Field 1 and Check Table Field 2 field).This is the
actual field that will be loaded into the target table

Lookup Table Where Clause

Displays the where clause used to filter values in the lookup table
column to restrict the values used in the lookup table.
