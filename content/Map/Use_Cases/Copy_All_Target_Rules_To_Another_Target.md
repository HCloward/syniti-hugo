+++
title = 'Copy All Target Rules to Another Target'
solution = 'Migration'
+++

# Copy All Target Rules to Another Target

A user can copy all rules from a target to share them across waves that
use the same target for migration. Using this feature, a user can seed
the target rules from one wave into another at the Wave, Process Area,
Object, Target level.

To copy all Target Rules to another target in Map:

1.  [Access Map](../Config/Access_Map.htm).

2.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch_map.htm)* page.

3.  Click **Vertical View** for a Target.

4.  Click the **Copy To** icon on the Page toolbar.

5.  Click **Edit**.
    
    *[View the field descriptions for the Target Rule Copy To
    page](../Page_Desc/Target_Rule_Copy_To.htm)*

6.  Select the expanded name of the source object that contains the rule
    to be copied from the **Copy To Source Database Object ID** list
    box.

7.  Click the **Activate Inactive Fields In Copy To Target** check box
    to enable it, which activates the inactive fields in the Copy To
    Target Database Object ID (if the Source has active fields).

8.  Click the **Initialize All Mappings In Copy To Target** check box to
    enable it, which resets the Mapping Status and all Field Mapping
    files to NULL. The copy process then loads the new mappings.
    
    **NOTE:** If a Copy To field had an Action and the Copy From field
    was blank, the Action field will have a value of NULL.

9.  Click **Save**.

10. Click the **Copy To** icon on the Page toolbar to finalize the copy
    process.
