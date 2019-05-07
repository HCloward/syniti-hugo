+++
title = 'Refresh Lookup Tables'
solution = 'Migration'
+++

# Refresh Lookup Tables

When changes to lookup tables are saved in Target Design, those changes
are automatically synced to Map.

**NOTE:** To refresh lookup table values, the tables must be active and
the lookup table’s Type must be set to Configuration.

To refresh check table values for the Target and the Source in Map:

1.  Select **Map** on the Context bar.
2.  Click the **Targets** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch_map.htm)* page.
3.  Click the **Mappings** icon for a Target.
4.  Click the **LOOKUP** link for a mapping with an action of XRef or
    RuleXref.
5.  Click the **Refresh** icon to refresh Target values; a confirmation
    message displays.
6.  Click **OK**.
7.  Click the **Sources** icon on the *[Value Mapping
    (Config)](../Page_Desc/Value_Mapping_Config_H.htm)* page.
8.  Click the **Value Mappings** icon for the SOURCE – CHECK TABLE
    combination.
9.  Click the **Refresh** icon for the Source tables; a confirmation
    message displays.
10. Click **OK**.

 

**NOTE**: After loading Source values into a lookup table in Map, only
those Source values that are to be mapped (as in, only those fields for
which a rule has been created) are retained in the lookup table when the
Target is processed. Unmapped Source value fields are deleted.

Lookup tables are primarily configured in Target Design. Refer to [Set
up Lookup
Tables](../../Design/Use_Cases/Set_up_a_Simple_Lookup_Table.htm) for
more information. A few settings must be updated in Map. Select
Configuration \> Value Mapping (Config) to access to edit settings for
lookup tables.
