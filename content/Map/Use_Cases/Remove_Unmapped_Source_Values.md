# Remove Unmapped Source Values

While value mapping, if a Source has many values that are not used (as
in, only the values in the Target table must be value mapped), a
Migration Developer can remove them before importing the Target table.
Removing unused Source values allows a user to more easily value map, as
only relevant Source values display.

Before this task can be performed, the lookup table must have been
[created or imported](../../Design/Use_Cases/Set_up_Lookup_Tables.htm)
and a mapping with the [Xref](Xref.htm) or [RuleXref](Rule_Xref.htm)
action must be created.

To remove the unused Source values:

1.  Click <span style="font-weight: bold;">Map</span> in the Context
    bar.

2.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch_map.htm)* page.

3.  Click the <span style="font-weight: bold;">Mappings</span> icon for
    a Target.

4.  Click the link for a lookup table used in the value mapping in the
    <span style="font-weight: bold;">LOOKUP</span> field.
    
    **NOTE:** This type of mapping uses an Xref or RuleXref action.

5.  Click the <span style="font-weight: bold;">Sources</span> icon.

6.  Click the **Vertical View** icon for the Source used in the value
    mapping.

7.  Click the <span style="font-weight: bold;">Remove Values</span>
    icon.
    
    **NOTE:** All values are removed in the Source field (stored in the
    Source data source) that have not yet been value mapped to a Target
    table. Use this feature only if the remaining values in the Source
    field should not be mapped to the Target field (as in, when mapping
    a field with an Xref action and processing objects in Transform.)

8.  Click the <span style="font-weight: bold;">Target Table
    Import</span> icon.

The import loads only those values that must be value mapped.
