+++
title = 'View Field Mapping History'
solution = 'Migration'
+++

# View Field Mapping History

On the *[Field Mapping History](../Page_Desc/Field_Mapping_History)*
page, a user can view changes made to a selected field’s mapping. A new
record is created on this page when:

  - The mapper submits a mapping on the *[Field
    Mappings](../Page_Desc/Field_Mappings_H)* page.
  - A Developer approves or rejects a mapping on the *[Mapping
    Approval](../Page_Desc/Mapping_Approval_H)* page.
  - A mapper resets a mapping to update it if a Developer rejects the
    mapping.

If a field belongs to multiple field groups, changes for each of these
field groups also display.

**NOTE:** If a field has not yet been mapped (as in, both the Mapping
Status and the Rule Status are Pending Review), no records display for
the field on the *Field Mapping History* page.

**NOTE:** If the message regarding pending design changes displays next
to the *Field Mappings* page’s title, the field data is out of sync with
Target Design. Until Map and Target Design are synced, field mapping
history may not be accurate. Refer to [Sync Map and Target
Design](../../Design/Use_Cases/Sync_Map_and_Target_Design_TD) for
more information.

Mapping History is not tracked if an action is preformed outside of Map.
The following fields do not display any mapping history records on the
*Field Mapping History* page:

  - Sources of {Full Construction}
  - A field that has a complex or basic rule added in Target Design.  No
    mappings can be performed in Map and therefore no field mapping
    history records display.

To view mapping history for a field in Map:

1.  Click <span style="font-weight: bold;">Map</span> in the Context
    bar.
2.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch_map)* page.
3.  Click the <span style="font-weight: bold;">Mappings</span> icon for
    a Target.
4.  Select a field and click the
    <span style="font-weight: bold;">History</span> icon in the Page
    toolbar.
