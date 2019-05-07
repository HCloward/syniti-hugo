+++
title = 'Sync Map and Target Design'
solution = 'Migration'
+++

# Sync Map and Target Design

When changes have been made that require a sync, the message Pending
Design Changes displays for the Target on the
<span style="font-style: italic;">[Design
Status](Set_Design_Status.htm)</span> page in Target Design. On the
<span style="font-style: italic;">[Targets](../Page_Desc/Targets_H_Design.htm)</span>
page, a Pending Design Changes link displays for the Target. Click the
link to view a list of changes for the selected Target.

The Pending Design Changes message also displays in Map on the
<span style="font-style: italic;">[Target
Sources](../../Map/Page_Desc/Target_Sources_H_Map.htm)</span> and
<span style="font-style: italic;">[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H.htm)</span> page.

For example, a user creates a Target table, ttMARA, in Target Design,
then clicks the Sync To Map icon to push the Target, fields and Source
to Map.

A user then adds a field and removes a field from the ttMARA Target on
the <span style="font-style: italic;">[Target
Fields](../Page_Desc/Target_Fields_H_Target_Design.htm)</span> page in
Target Design.

At this point, when the ttMARA Target is selected on the
<span style="font-style: italic;">[Targets](../../Map/Page_Desc/Targets_H_Map.htm)</span>
page, the message Pending Design Changes displays for the Target. The
user can click this link to view the pending changes (the field that was
removed and the field that was added) on the
<span style="font-style: italic;">[Target Design Pending
Changes](../Page_Desc/Target_Design_Pending_Changes.htm)</span> page.

The Pending Design Changes message also displays on the
<span style="font-style: italic;">Design Status</span> page in Target
Design and on the <span style="font-style: italic;">Target
Sources</span> and <span style="font-style: italic;">Field
Mappings</span> page in Map.

The user must then run the Sync process in Target Design or Map.

<span style="font-weight: bold;">NOTE</span>: In Target Design and Map,
the Sync to Map icon is active when a selected Target’s Design Status is
In Design and Design Finished. The icon is disabled if the Design Status
is Inactive or Complete.

**NOTE**: If changes are pending to a Target design:

  - The Design Status cannot be changed to Design Finished or Complete
    until the sync process runs.
  - The Design Status can be moved to In Design.

Refer to [Set the Design Status](Set_the_Design_Status.htm) for more
information.

**NOTE**: When the Sync process runs, if a Target Source is {Full
Construction}, AutoGen runs to create the page and underlying tables and
views in Construct. Refer to [Full Construction and Enhanced
Construction](../../Construct/Use_Cases/Full_Construction_and_Enhanced_Construction.htm)
for more information.

**NOTE**: The Design Status is not updated by the Sync process.

To sync Target Design and Map in Target Design:

1.  Click **Design** in the Context bar.

2.  Click the **Targets**icon on the *[Design](../Page_Desc/Design.htm)*
    page.

3.  Select a Target that needs to be synced on the *Targets* page.

4.  Click the **Sync to Map** icon on the Page toolbar of the *Targets*
    page.
    
    **NOTE**: This icon is disabled if the Target selected on the
    *Targets* page is in Complete or Inactive status.

5.  Click the <span style="font-weight: bold;">Fields</span> icon for a
    Target and then click the <span style="font-weight: bold;">Sync to
    Map</span> icon on the <span style="font-style: italic;">Targets
    Fields</span> page.
    
    **NOTE**: Only the Target selected on the *Targets* page is synced.

To sync Target Design and Map in Map:

1.  Select **ProcessArea** in the *Navigation* pane.

2.  Click the **Sources**icon for a Process Area.
    
    OR
    
    Click the **Targets** icon for a Process area and then click the
    **Mappings** icon for a Target

3.  Click the **Sync From Target Design** icon in the Page toolbar.

New fields that are activated on the *Target Fields* page in Target
Design are loaded into Map

  - Edits to active fields, such as changes in Key status or lookup
    tables, are loaded into Map.
  - Fields that are deactivated on the *Target Fields* page in Target
    Design and do not have a Rule Status of Complete on the Field
    Mappings page in Map are removed from Map.
  - Fields that are deactivated on the *Target Fields* page in Target
    Design but have a Mapping Status and Rule Status of Complete in Map
    are reset. In Transform, these fields are updated to Inactive
    status.
  - Fields that are deleted in Target Design are removed from Map unless
    those fields are key fields. Key fields are not removed from Map,
    even when deleted in Target Design.
  - Relationships added on the
    <span class="msoIns" style="font-style: italic;">[Target Dependency
    Relationship](../Page_Desc/Target_Dependency_Relationship.htm)</span>
    page are loaded into Map.

If the original mapping action created a rule in Transform, what happens
to that rule when it is reset in Map is determined by a parameter set in
Console on the Map tab of the *Parameters* page. In the Reset Transform
Rule list box, the following options are available:

  - **Delete Transform Rule** – The rule Map created during the mapping
    process and registered in Transform is deleted when the mapping is
    reset in Map. The rule is deleted from the database and its
    registrations are removed from Transform.
  - **Deactivate Transform Rule** – The status of the rule Map created
    during the mapping process and registered in Transform is changed to
    Inactive in Transform when the mapping is reset in Map.
  - **Ignore Transform Rule** – The rule Map created during the mapping
    process and registered in Transform is not affected by the reset.
