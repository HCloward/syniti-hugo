+++
title = 'Perform Value Mapping Overview'
solution = 'Migration'
+++

# Perform Value Mapping Overview

In value mapping, an individual value in a Source field is configured to
be converted to a value that the Target system will accept in the Target
field. For example, if two large companies merge, they may want to
convert the Legacy Org Numbers first and then value map to the new Org
numbers (in an Org check table) in the Target ERP system.

The field and value that must be value mapped in the Target system are
stored in check tables, also called lookup tables.

Besides updating value mappings in the UI as described in this topic, a
user can also:

  - Perform value mapping automatically, if the Source system and Target
    system are identical, value mapping can be performed automatically.
    On the *[Value Mapping](../Page_Desc/Value_Mapping)* page, click
    **Auto Map By Description** or **Auto Map By Value** in the Page
    toolbar.

  - Use Excel Integration to download a spreadsheet that users can
    update with value mapping values. Ensure Bulk Execution is enabled
    on the *[Value Mapping (Legacy to
    Target)](../Page_Desc/Value_Mapping_Legacy_to_Target_H)* page.
    Once data entry is complete, import that data into the DSP. Refer to
    [Use Excel
    Integration](../../../Platform/Excel_Int/Use_Excel_Integration)
    for more information.

**NOTE:** The RuleXref action must be used with a lookup table that has
multiple key fields. This allows missing values in the Target table to
be inserted into the Value Mapping table. The Xref action can only be
used with a lookup table that has a single key field. If the Target
Lookup table is a multiple key table, the Value Mapping process
concatenates Target values from the multiple key fields into a single
field. To map fields on a multiple key lookup table, use the RuleXref
action for the field to be mapped on the
<span style="font-style: italic;">Field Mappings</span> page. RuleXref
concatenates Source values and is the recommended Migration Solution
process to load the values correctly into the Value Mapping process.

<span style="font-weight: bold;">NOTE:</span> When mapping fields on a
multiple key lookup table, concatenate the fields with a ":" separator,
for example, field1:field 2.

<span style="font-weight: bold;">NOTE:</span> A lookup table is
registered as a Source table with a status of Documentation and a rule
priority offset of 50000 so that it is sorted last. Documentation
Sources are not processed but are a reference item to see all the
sources of data.

<span style="font-weight: bold;">NOTE:</span> The Source table and
Source field for the check table for the Rule Xref action are not
automatically set. They must be entered on the
<span style="font-style: italic;">Vertical</span> View of the [Legacy
Value (Source Table
Fields)](../Page_Desc/Legacy_Value_Source_Table_Fields_H) page.

The steps in the value mapping process are:

1.  Set up Lookup Tables in Target Design or import check tables with a
    System Type import. Refer to [Set up Lookup
    Tables](../../Design/Use_Cases/Set_up_a_Simple_Lookup_Table) or
    [Import Target Design from a System
    Type](../../Design/Use_Cases/Import_from_a_System_Type) for more
    information.
2.   [Refresh lookup tables or change configuration
    settings](Refresh_Lookup_Tbls) as needed in Map.
3.  [Perform value mapping](Perform_Value_Mapping) in Map.

This section contains the following topics:

  - [Designate a System for a Check
    Table](Designate_a_System_for_Check_Table)
  - [Refresh Lookup Tables](Refresh_Lookup_Tbls)
  - [Refresh Target and Legacy
    Values](Refresh_Target_and_Legacy_Values)
  - [Remove Unmapped Source Values](Remove_Unmapped_Source_Values)
  - [Perform Value Mapping](Perform_Value_Mapping)
  - [View the Source Tables and Fields Mapped to a Lookup
    Table](View_the_Source_Tables_and_Fields_Mapped_to_a_Lookup_Table)
  - [Value Map Target Fields for Multiple Source
    Systems](Value_Map_Target_Fields_from_Mulitple_Source_Systems)
