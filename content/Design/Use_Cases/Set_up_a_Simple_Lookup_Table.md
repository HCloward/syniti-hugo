+++
title = 'Set up a Simple Lookup Table'
solution = 'Migration'
+++

# Set up a Simple Lookup Table

A simple lookup table contains one key.

Refer to [Set up Lookup Tables](Set_up_Lookup_Tables.htm) for more
information.

A lookup table that already exists can be edited or a lookup table can
be added. The process is the same.

<span style="font-weight: bold;">NOTE</span>: The RuleXref action must
be used with a lookup table that has multiple key fields. This will
allow missing values in the Target table to be inserted into the Value
Mapping table. The Xref action can only be used with a lookup table that
has a single key field. If the Target Lookup table is a multiple key
table, the Value Mapping process will concatenate Target values from the
multiple key fields into a single field. To map fields on a multiple key
lookup table, use the RuleXref action for the field to be mapped on the
<span style="font-style: italic;">[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H.htm)</span> page.
RuleXref concatenates Source values and is the recommended Migration
Solution process to load the values correctly into the Value Mapping
process.

<span style="font-weight: bold;">NOTE</span>: A description for the
Lookup Table Value table can be added on the
<span style="font-style: italic;">[Target Lookup
Table](../Page_Desc/Target_Lookup_Table_H.htm)</span> page's
<span style="font-style: italic;">Vertical</span> View in the
Description field.

To add or edit a simple lookup table in Target Design:

1.  Select **Configuration \> Lookup Table Setup** in the *Navigation*
    pane.

2.  Click **Edit** or **Add**
    
    .*[View the field descriptions for the Target Lookup Table
    page.](../Page_Desc/Target_Lookup_Table_H.htm)*

3.  Enter the name of the table that contains the values that are used
    in value mapping in the **VALUE** **TABLE NAME** field.
    
    **NOTE**: If editing a lookup table, this name is already provided.

4.  Select an option in the
    **<span id="Lookup Table Type" class="popUpLink">TYPE</span>** list
    box.

5.  Enter the key field in the lookup table in the **VALUE TABLE COLUMN
    1** field. 

6.  Enter the name of the table that stores the descriptions for the
    values in the value table in the **DESCRIPTION TABLE NAME** field.
    
    **NOTE**: This field displays in Map on the *Vertical* View of the
    *[Value Mapping
    (Config)](../../Map/Page_Desc/Value_Mapping_Config_H.htm)* page.

7.  Enter the name of the column that stores the descriptions for the
    values in the value table in the **DESCRIPTION TABLE COLUMN** field.

8.  Click **Save**.
