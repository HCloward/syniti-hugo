+++
title = 'Update Unmapped Fields to NotUsed'
solution = 'Migration'
+++

# Update Unmapped Fields to NotUsed

## <span id="Update_Unmapped_Target_Source_Fields"></span>Update Unmapped Target Source Fields

If there are several unmapped fields (i.e., where the ACTION field is
blank) in a source that need to be set to NotUsed, use the Auto Update
Not Used feature.

To automatically update unmapped fields to NotUsed in Map:

1.  Click **ProcessArea** in the *Navigation* pane.

2.  Click the **Targets**icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch_map.htm)* page.

3.  Click the **Sources** icon for a TARGET ID.

4.  Click the **Vertical View** icon for the Target Source.

5.  Click the **Auto Update Not Used** icon on the Page toolbar; a
    confirmation message displays.

6.  Click
**OK**.

## <span id="Update_Add_Row_and_Update_Row_Source_Fields"></span>Update Unmapped Add Row and Update Row Source Fields

An option in Console allows Map to update the ACTION field for Add Row
and Update Row Sources to NotUsed once a field is mapped in another Add
Row or Update Row Source. This option only updates actions that have not
been set (as in, the ACTION field is blank) on the
<span style="font-style: italic;">[Field
Mappings](../Page_Desc/Field_Mappings_H.htm)</span> page in Map.

If an Add Row or Update Row Source is mapped to another Add Row or
Update Row Source in Map, the Auto Set Not Used for Multiple Sources
setting on the *[Parameters](../../Console/Page_Desc/Parameters.htm)*
page in Console controls how Map updates an action that is not set. Map
updates the ACTION field on the *Field Mappings* page once the mapping
is saved.

The Auto Set Not Used for Multiple Sources list box has three options:

  - <span style="font-weight: bold;">None</span> — The values in the
    ACTION field for the Add Row or Update Row Sources are not changed
    in other Sources.

  - <span style="font-weight: bold;">Primary and Secondary Source</span>
    — When a mapping is saved in an Add Row or Update Row Source, Map
    updates the ACTION field for actions that are not set with NotUsed.

  - <span style="font-weight: bold;">Secondary Source Only</span> — When
    a mapping is saved for an Add Row or Update Row Source, only the
    Update Row Source ACTION field for all other mappings are set to
    NotUsed.  The Add Row Source’s action remains unchanged.

<span style="font-weight: bold;">NOTE</span>: An action of NotUsed can
be updated after it has been set.

To set this option in Console:

1.  Select <span style="font-weight: bold;">Advanced Configuration \>
    Parameters</span>in the
    <span style="font-style: italic;">Navigation</span>pane.

2.  Click the <span style="font-weight: bold;">Map</span> tab.

3.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Parameter's page in
    Console.](../../Console/Page_Desc/Parameters.htm)

4.  Select an option from the <span style="font-weight: bold;">Auto Set
    Not Used for Multiple Sources</span> list box.

5.  Click <span style="font-weight: bold;">Save</span>.
