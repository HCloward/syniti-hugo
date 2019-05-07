+++
title = 'Copy a Target Source to Another Target'
solution = 'Migration'
+++

# Copy a Target Source to Another Target

Once a Source is configured in Target Design and synced to Map, field
mappings and field groups from a Source can be copied to a new Source to
expedite the mapping process. When a Source is copied, all mappings are
copied where the Target and Source tables match.

**NOTE**: The copy process <span style="color: #ff0000;">cannot be
performed</span> until:

  - The Source has been added in Target Design
  - The Target associated with the Target Source has been synced with
    Map

Refer to [Add a
Source](../../Design/Use_Cases/Assign_a_Source_to_a_Target.htm) and
[Sync Target Design and
Map](../../Design/Use_Cases/Sync_Map_and_Target_Design_TD.htm) for more
information.

When a Source is copied, the mapping status and rule status for all
copied mappings is Pending Review. Refer to [Mapping Status and Rule
Status](Mapping_Status_and_Rule_Status.htm) for more information.

To copy a Source in Map:

1.  [Access Map](../Config/Access_Map.htm).

2.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch_map.htm)* page.

3.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.

4.  Click **Vertical View** for a Target Source.

5.  Click the **Copy To** icon on the Page toolbar.

6.  Click **Edit**.
    
    [*View the field descriptions for the Target Source Copy To
    page*](../Page_Desc/Target_Source_Copy_To.htm)

7.  Select an expanded name of the Source, which includes the Wave,
    Process Area, Object and Target from the **Copy To Source Database
    Object ID** list box.

8.  Click the **Activate Inactive Fields In Copy To Target** check box
    to enable it, which activates the inactive fields in the Copy To
    Source Database Object ID (if the Source has active fields).

9.  Click the **Initialize All Mappings In Copy To Target** check box to
    enable it, which resets the Mapping Status and all Field Mapping
    files to Null. The copy process then loads the new mappings.
    
    **NOTE:** If a Copy To field had an Action and the Copy From field
    was blank, the Action field will have a value of NULL.

10. Click **Save**.

11. Click the **Copy To** icon on the Page toolbar to finalize the copy
    process.
