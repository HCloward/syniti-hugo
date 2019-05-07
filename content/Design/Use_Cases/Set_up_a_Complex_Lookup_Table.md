+++
title = 'Set up a Complex Lookup Table'
solution = 'Migration'
+++

# Set up a Complex Lookup Table

A complex lookup table contains a multiple part key.

Refer to [Set up Lookup Tables](Set_up_Lookup_Tables.htm) for more
information.

**NOTE**: A lookup table can be added in Target Design with up to five
key fields. If the table requires more than five key fields, a view must
be written.

**NOTE**: If the Target system is Oracle, a view must be written. A
Target lookup table for an Oracle Target cannot be created using the
*[Target Lookup Table](../Page_Desc/Target_Lookup_Table_H.htm)* page.

<span style="font-weight: bold;">NOTE</span>: The RuleXref action must
be used with a lookup table that has multiple key fields. This allows
missing values in the Target table to be inserted into the Value Mapping
table. The Xref action can only be used with a lookup table that has a
single key field. If the Target Lookup table is a multiple key table,
the Value Mapping process concatenates Target values from the multiple
key fields into a single field. To map fields on a multiple key lookup
table, use the RuleXref action for the field to be mapped on the
<span style="font-style: italic;">Field Mappings</span> page. RuleXref
concatenates Source values and is the recommended Migration Solution
process to load the values correctly into the Value Mapping process.

<span style="font-weight: bold;">NOTE</span>: When mapping fields on a
multiple key lookup table, concatenate the fields with a ":" separator,
for example, field1:field 2.

<span style="font-weight: bold;">NOTE</span>: A description for the
Lookup Table Value table can be added on the
<span style="font-style: italic;">Target Lookup Table</span> page's
<span style="font-style: italic;">Vertical</span> View in the
Description field.

A lookup table that already exists can be edited, or a lookup table can
be added. The process is the same.

To configure a complex lookup table (one with a multipart key) in Target
Design:

1.  Select **Configuration \> Lookup Table Setup** in the *Navigation*
    pane.

2.  Click **Edit** or **Add**.
    
    *[View the field descriptions for the Target Lookup Table
    page](../Page_Desc/Target_Lookup_Table_H.htm)*

3.  Enter the name of the table that contains the values that are used
    in value mapping in the **VALUE TABLE NAME** field.
    
    **NOTE**: If editing a lookup table, this name is already provided.

4.  Select an option in the **TYPE** list box.

5.  Enter the first key in a value table with a multipart key in the
    **VALUE TABLE COLUMN 1** field.

6.  Enter the second key in a value table with a multipart key in the
    **VALUE TABLE COLUMN 2** field.
    
    **NOTE**: Additional columns can be added on the *Vertical* View.

7.  Enter the column on the Value Table that stores the Client or Tenant
    of the data in the **VALUE TABLE CLIENT COLUMN** field.
    
    **NOTE**: This field is used with SAP only.

8.  Enter the name of the table that stores the descriptions for the
    values in the value table in the **DESCRIPTION TABLE NAME** field.
    
    **NOTE**: This field displays in Map on the *Vertical* View of the
    *[Value Mapping
    (Config)](../../Map/Page_Desc/Value_Mapping_Config_H.htm)* page
    (Configuration \> Value Mapping (Config)).

9.  Enter the name of the column that stores the descriptions for the
    values in the value table in the **DESCRIPTION TABLE COLUMN** field.

10. Enter the key column on the Description table used to uniquely
    identify values if the Description table key is different from the
    Value table's key column in the **DESCRIPTION TABLE KEY COLUMN**
    field.
    
    **NOTE**: This field is used with the lookup table T006.
    
    **NOTE**: If this field is blank, the Description Table Key uses the
    Value Table Key.

11. Enter the column on the Description Table that stores the Client or
    Tenant of the data in the **DESCRIPTION TABLE CLIENT COLUMN** field.
    
    **NOTE**: This field is used with SAP only.

12. Enter the column on the Description Table that stores the language
    identifier column in the **DESCRIPTION TABLE LANGUAGE COLUMN**
    field.
    
    **NOTE**: This field is used with SAP only.

13. Click **Save**; the *Vertical* View displays.

14. Select the column containing the value to use if more than one value
    table column is set for the value table (as in, there is data in the
    **VALUE TABLE COLUMN 1** and **VALUE TABLE COLUMN 2** fields and so
    on) in the **MULTI VALUE FIELD LOOKUP TABLE VALUE COLUMN** list box.
    
    **NOTE**: This is the actual field that will be loaded into the
    Target table.

15. Enter the where clause used to filter values in the value table
    column to restrict the values used in the lookup table in the
    **WHERE CLAUSE** field, if needed.

16. Click **Save**.
