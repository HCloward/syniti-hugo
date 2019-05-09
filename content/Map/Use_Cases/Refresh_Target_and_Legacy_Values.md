+++
title = 'Refresh Target and Legacy Values'
solution = 'Migration'
+++

# Refresh Target and Legacy Values

In value mapping, an individual value in a Source field is configured to
be converted to a value that the Target system accepts in the Target
field.

These values display in the list boxes Legacy Value and Target Value on
the [Value Mapping (Legacy to
Target)](../Page_Desc/Value_Mapping_Legacy_to_Target_H) page. If no
options display in these list boxes (as in, the only option in the list
box is None), the Target values and legacy values must be refreshed on
the [Wave Check Table
Refresh](../Page_Desc/Wave_Lookup_Table_Refresh) page.

<span style="font-weight: bold;">NOTE</span>: Lookup tables are either
created in Target Design or imported into Target Design with a System
Type. When changes to lookup tables are saved in Target Design, those
changes are automatically synced to Map. Refer to [Set up Lookup
Tables](../../Design/Use_Cases/Set_up_Lookup_Tables) for more
information.

Prior to performing the refresh, ensure:

  - The selected Wave is active.
    (<span style="font-weight: bold;">Console \> Waves</span>; Enable
    the <span style="font-weight: bold;">ACTIVE</span> check box).
  - The Target System and Client are the correct ones to use for value
    mapping for the selected Wave
    (<span style="font-weight: bold;">Console \> Waves</span>; click
    <span style="font-style: italic;">Vertical</span> View).
  - The lookup tables have been downloaded in Collect. Refer to [Refresh
    Tables](../../../Platform/Collect/Use_Cases/Refresh_Tables) for
    more information.
  - The lookup table is active and the lookup table’s type is
    Configuration.

To refresh the values in Map:

1.  Select <span style="font-weight: bold;">Configuration \> Wave Check
    Table Refresh</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Select the Wave that contains the lookup tables.
    
    **NOTE:** Ensure the <span style="font-weight: bold;">ACTIVE</span>
    check box is checked.

3.  Click the <span style="font-weight: bold;">Refresh Target
    Values</span> icon or the <span style="font-weight: bold;">Refresh
    Legacy Values</span> icon in the Page toolbar; a confirmation
    message displays.

4.  Click <span style="font-weight: bold;">OK</span>.

The list boxes Legacy Value and Target Value on the [Value Mapping
(Legacy to Target)](../Page_Desc/Value_Mapping_Legacy_to_Target_H)
page display the legacy values and/or the Target values used in value
mapping. Refer to [Perform Value
Mapping](Perform_Value_Mapping_Overview) for more information.

To refresh values for a single Target or Source, refer to [Refresh
Lookup Tables](Refresh_Lookup_Tbls) for more information.
