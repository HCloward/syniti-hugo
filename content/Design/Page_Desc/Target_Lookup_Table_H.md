+++
title = 'Target Lookup Table H'
solution = 'Migration'
+++

# Target Lookup Table H

[Target Lookup Table V](Target_Lookup_Table_H#Target_Lookup_Table_V)

<div class="use">

Use this page to [Set up Lookup
Tables](../Use_Cases/Set_up_Lookup_Tables).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Select <span style="font-weight: bold;">Design </span>in the Context
    bar.
3.  Select <span style="font-weight: bold;">Configuration \> Lookup
    Table Setup</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Value Mapping (Config)</p></td>
<td><p>Click to open the <em><a href="../../Map/Page_Desc/Value_Mapping_Config_H">Value Mapping (Config)</a></em> page in Map to refresh lookup table values after changers to configuration of a lookup table.</p></td>
</tr>
<tr class="odd">
<td><p>VALUE TABLE NAME</p></td>
<td><p>Displays the name of the table that contains the values used in the lookup table.</p></td>
</tr>
<tr class="even">
<td><p><span id="Lookup Table Type" class="popUpLink">TYPE</span></p></td>
<td><p>Displays an option indicating whether fields in the lookup table should be value mapped.</p></td>
</tr>
<tr class="odd">
<td><p>VALUE TABLE COLUMN 1</p></td>
<td><p>Displays the first key in a value table with a multipart key.</p>
<p>Displays the key in a value table with a single key.</p>
<p>If more than one Value Table Column is entered for a table, one column name must be selected in the MULTI FIELD LOOKUP TABLE VALUE COLUMN on the <em>Vertical</em> View because tables with multipart keys require a column to be selected for the update rule.</p>
<p>For example, a lookup table for a city must also include the city’s state. In this case, the Value Table Column1 field contains the State column and the Value Table Column2 field contains the City column. The MULTI FIELD LOOKUP TABLE VALUE COLUMN uses the City column as the key, as the City column is what is being value mapped.</p>
<p>This value displays in Map in the Value Field1 field on the <span style="font-style: italic;">Vertical</span> View of the <span style="font-style: italic;"><a href="../../Map/Page_Desc/Value_Mapping_Config_H">Value Mapping (Config)</a></span> page.</p></td>
</tr>
<tr class="even">
<td><p>VALUE TABLE COLUMN 2</p></td>
<td><p>Displays the second key in a value table with a multipart key.</p>
<p>If more than one Value Table Column is entered for a table, one column name must be selected in the MULTI FIELD LOOKUP TABLE VALUE COLUMN on the <em>Vertical</em> View because tables with multipart keys require a column to be selected for the update rule.</p>
<p>This value displays in Map in the Value Field2 field on the <span style="font-style: italic;">Vertical</span> View of the <span style="font-style: italic;"> <a href="../../Map/Page_Desc/Value_Mapping_Config_H">Value Mapping (Config)</a></span> page.</p></td>
</tr>
<tr class="odd">
<td><p>VALUE TABLE CLIENT COLUMN</p></td>
<td><p>Displays the column on the value table that stores the Client or Tenant of the data. Used with SAP only.</p></td>
</tr>
<tr class="even">
<td><p>MULTI VALUE FIELD LOOKUP TABLE VALUE COLUMN</p></td>
<td><p>Displays the column containing the value to use if more than one value table column is set for the value table (for example, there is data in the VALUE TABLE COLUMN 1 and VALUE TABLE COLUMN 2 fields). This is the actual field that will be loaded into the Target table.</p>
<p><strong>NOTE</strong>: This field is updated on the <em>Vertical</em> View.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION TABLE NAME</p></td>
<td><p>Displays the name of the table that stores the descriptions for the values in the value table.</p>
<p><strong>NOTE</strong>: This field displays in Map on the Vertical View of the <span style="font-style: italic;"><a href="../../Map/Page_Desc/Value_Mapping_Config_H">Value Mapping (Config)</a></span> page.</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION TABLE COLUMN</p></td>
<td><p><span>Displays the name of the column that stores the descriptions for the values in the value table </span>for a table with a single key.</p>
<p>This value displays in Map in the Description Field field on the <span style="font-style: italic;">Vertical</span> View of the <span style="font-style: italic;"> <a href="../../Map/Page_Desc/Value_Mapping_Config_H">Value Mapping (Config)</a></span> page.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION TABLE KEY COLUMN</p></td>
<td><p>Displays the key column on the Description table used to uniquely identify values if the Description table key is different from the value table's key column.</p>
<p>This field is used by the T006 check table.</p>
<p>If this field is blank, the Description Table Key uses the Value Table Key.</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION TABLE LANGUAGE COLUMN</p></td>
<td><p>Displays the column on the Description Table that stores the language identifier column. Used with SAP only.</p></td>
</tr>
</tbody>
</table>

##  

## <span id="Target_Lookup_Table_V"></span>Target Lookup Table V

[Target Lookup Table H](Target_Lookup_Table_H)

<div class="use">

Use this page to [Set up Lookup
Tables](../Use_Cases/Set_up_Lookup_Tables).

</div>

Field

Description

Value Table

 

<span id="Lookup Table Type" class="popUpLink">Type</span>

Displays an option indicating whether fields in the check table should
be value mapped.

Value Table Name

Displays the name of table that contains the values used in the lookup
table.

Description

Displays a description of the lookup table. This field may be populated
when a System Type was imported into Target Design, or may have been
updated by a user. The description displays in Map on the
<span style="font-style: italic;">[Value
Mapping](../../Map/Page_Desc/Value_Mapping)</span> page.

Value Table Column 1

Displays the first key in a value table with a multipart key.

If more than one Value Table Column is entered for a table, one column
name must be selected in the MULTI FIELD LOOKUP TABLE VALUE COLUMN
because tables with multipart keys require a column to be selected for
the update rule.

For example, a lookup table for a city must also include the city’s
state. In this case, the Value Table Column1 field contains the State
column and the Value Table Column2 field contains the City column. The
MULTI FIELD LOOKUP TABLE VALUE COLUMN uses the City column as the key,
as the City column is what is being value mapped.

Value Table Column 2

Displays the second key in a value table with a multipart key.

If more than one Value Table Column is entered for a table, one column
name must be selected in the MULTI FIELD LOOKUP TABLE VALUE COLUMN
because tables with multipart keys require a column to be selected for
the update rule.

This value displays in Map in the Value Field2 field on the
<span style="font-style: italic;">Vertical</span> View of
the<span style="font-style: italic;"> [Value Mapping
(Config)](../../Map/Page_Desc/Value_Mapping_Config_H)</span> page.

Value Table Column 3

Displays the third key in a value table with a multipart key.

If more than one Value Table Column is entered for a table, one column
name must be selected in the MULTI FIELD LOOKUP TABLE VALUE COLUMN
because tables with multipart keys require a column to be selected for
the update rule.

This value displays in Map in the Value Field3 field on the
<span style="font-style: italic;">Vertical</span> View of the
<span style="font-style: italic;">[Value Mapping
(Config)](../../Map/Page_Desc/Value_Mapping_Config_H)</span> page.

Value Table Column 4

Displays the fourth key in a value table with a multipart key.

If more than one Value Table Column is entered for a table, one column
name must be selected in the MULTI FIELD LOOKUP TABLE VALUE COLUMN
because tables with multipart keys require a column to be selected for
the update rule.

This value displays in Map in the Value Field4 field on the
<span style="font-style: italic;">Vertical</span> View of the
<span style="font-style: italic;">[Value Mapping
(Config)](../../Map/Page_Desc/Value_Mapping_Config_H)</span> page.

Value Table Column 5

Displays the fifth key in a value table with a multipart key.

If more than one Value Table Column is entered for a table, one column
name must be selected in the MULTI FIELD LOOKUP TABLE VALUE COLUMN
because tables with multipart keys require a column to be selected for
the update rule.

This value displays in Map in the Value Field5 field on the *Vertical*
View of the <span style="font-style: italic;">[Value Mapping
(Config)](../../Map/Page_Desc/Value_Mapping_Config_H)</span> page.

**NOTE**: If a table requires more than 5 key fields, a view must be
written.

Value Table Client Column

Displays the column on the Value Table that stores the Client or Tenant
of the data. Used with SAP only.

Value Table Language Column

Displays the column on the Value Table that stores the language
identifier column. Used with SAP only.

Multi Value Field Lookup Table Value Column

Displays the column containing the value to use if more than one value
table column is set for the value table (e.g., there is data in the
VALUE TABLE COLUMN 1 and VALUE TABLE COLUMN 2 fields). This is the
actual field that will be loaded into the Target table.

Description Table

Description Table Name

Displays the name of the table that stores the descriptions for the
values in the value table.

**NOTE**: This field displays in Map in the Description Table field on
the <span style="font-style: italic;">Vertical</span> View of
the<span style="font-style: italic;"> Value Mapping (Config)</span> page
(Configuration \> Value Mapping (Config)).

Description Table Column

Displays the name of the column that stores the descriptions for the
values in the value table.

This field displays in Map in the Description Field field on the
<span style="font-style: italic;">Vertical </span> View of
the<span style="font-style: italic;">[Value Mapping
(Config)](../../Map/Page_Desc/Value_Mapping_Config_H)</span> page.

Description Table Key Column

Displays the key column on the Description table used to uniquely
identify values if the Description table key is different from the Value
table's key column.

This field is used by the T006 table.

If this field is blank, the Description Table Key uses the Value Table
Key.

Description Table Client Column

Displays the column on the Description Table that stores the Client or
Tenant of the data. Used with SAP only.

Description Table Language Column

Displays the column on the Description Table that stores the language
identifier column. Used with SAP only.

Filter Criteria

Where Clause

Displays the Where Clause used to filter values in the value table
column to restrict the values used in the lookup table.

Documentation

Comment

Displays user-entered text about the lookup table.

This field is for documentation purposes only.

Check Table System Type Table ID

Displays the name of the check table in the System Type upon which this
lookup table is based. This field may be populated when a System Type
was imported into Target Design, or may have been updated by a user.
