+++
title = 'Set up Lookup Tables'
solution = 'Migration'
+++

# Set up Lookup Tables

In value mapping, an individual value in a Source field in one table is
configured to be converted to a value stored in another table that the
target system will accept in the Target field. For example, if two large
companies merge, they may want to convert the Legacy Org Numbers first
and then value map to the new Org numbers (in an Org check table) in the
Target ERP system.

Refer to [Perform Value
Mapping](../../Map/Use_Cases/Perform_Value_Mapping_Overview.htm) for
more information.

The field and value that must be value mapped are stored in check
tables, also called lookup tables.

Lookup tables for a Source can be added in Target Design:

  - Manually by adding the tables and fields on the *[Target Lookup
    Table](../Page_Desc/Target_Lookup_Table_H.htm)* page in Target
    Design
  - Automatically on import, when a System Type that contains the lookup
    table is imported into Target Design. Check tables are stored in
    System Types, which are created in Common. Refer to [System
    Types](../../../Platform/Common/Use_Cases/System_Types_Overview.htm)
    in Common for more information.

Lookup tables are automatically synced to Map when the lookup table is
saved.

<span style="font-weight: bold;">NOTE</span>: A lookup table is
registered as a Source table with a status of Documentation and a rule
priority offset of 50000 so that it is sorted last. Documentation
sources are not processed but are a reference item to see all the
sources of data.

**NOTE**: If a Wave is copied in Console, the lookup tables are also
copied.

A simple lookup table contains one key. A complex lookup table contains
a multiple part key.

Refer to [Set up a Simple Lookup
Tables](Set_up_a_Simple_Lookup_Table.htm) and [Set up a Complex Lookup
Table](Set_up_a_Complex_Lookup_Table.htm) for more information.

**NOTE**: A lookup table can be added in Target Design with up to five
key fields. If the table requires more than five key fields, a view must
be written.

**NOTE**: If the Target system is Oracle, a view must be written. A
Target lookup table for an Oracle Target cannot be created using the
*Target Lookup Table* page.

A lookup table that already exists can be edited, or a lookup table can
be added. The process is the same.
