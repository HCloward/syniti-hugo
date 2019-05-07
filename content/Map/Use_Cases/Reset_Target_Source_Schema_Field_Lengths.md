+++
title = 'Reset Target Source Schema Field Lengths'
solution = 'Migration'
+++

# Reset Target Source Schema Field Lengths

If a Source was added in Target Design during a System Type import, and
the System Type tables for a Source contained an invalid length for a
column, use the Reset functionality to update a Source table with the
column’s correct length.

<span style="font-weight: bold;">NOTE</span>: Updates to field lengths
in System Types are not reflected in Target or Source tables until a
user clicks <span style="font-weight: bold;">Create</span> on the
<span style="font-style: italic;">[Targets](../Page_Desc/Targets_H_Map.htm)</span>
or the <span style="font-style: italic;">[Target
Sources](../Page_Desc/Target_Sources_H_Map.htm)</span> page. System
Types are defined and the field lengths are modified in Common. Refer to
[System
Types](../../../Platform/Common/Use_Cases/System_Types_Overview.htm) for
more information.

<span style="font-weight: bold;">NOTE</span>: To reset the length, the
user must know the table and field name with the invalid length for the
Target or Source.

To use the reset feature in Common:

1.  Select <span style="font-weight: bold;">System Types</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Tables</span> icon for
    the Target or Source System Type.

3.  Click the <span style="font-weight: bold;">Fields</span> icon for a
    table.

4.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the System Types - Table Fields
    page.](../../../Platform/Common/Page_Desc/System_Types_Table_Fields_H.htm)

5.  Enter a value in the <span style="font-weight: bold;">LENGTH</span>
    field.

6.  Click <span style="font-weight: bold;">Save</span>.

7.  Navigate to Map.

8.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the <span style="font-style: italic;">[Process Area
    Launch](../Page_Desc/Process_Area_Launch_map.htm)</span> page.

9.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.

10. Click <span style="font-weight: bold;">Vertical View</span> for a
    table for a Target or a Target Source.
    
    **NOTE:** Do not click the
    <span style="font-style: italic;">Vertical</span> View icon for a
    <span class="error" style="font-weight: bold;">\[Target
    Rules\]</span> Target Source.

11. Click the <span style="font-weight: bold;">Schema Columns</span>
    icon.

12. Click <span style="font-weight: bold;">Reset</span>; a confirmation
    message displays.

13. Click <span style="font-weight: bold;">OK</span>.
