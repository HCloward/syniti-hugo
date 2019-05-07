+++
title = "Set a Target's Design Status"
solution = 'Migration'
+++

# Set a Target's Design Status

The Design Status for a Target indicates where the Target design is in
the stages of the design process. To set the Design Status, click the
link in the DESIGN STATUS column for the Target on the
<span style="font-style: italic;">[Targets](../Page_Desc/Targets_H_Design.htm)</span>
page.

A Target’s Design Status can be changed. The current Design Status does
not restrict the ability to update the Design Status. For example, if a
Target is in Inactive status, it can be moved to Complete status. The
ability to add or edit a Target Contact for a Target is not affected by
the Target’s Design Status. A Target contact is for documentation
purposes only, and can be added or edited on the
<span style="font-style: italic;">Targets</span> page’s Vertical View.

The functionality available for Target configuration differs depending
on the Design Status.

<span style="font-weight: bold;">NOTE</span>: The ability to edit lookup
tables for a Target is not affected by the Target’s Design Status.

### In Design

When a Target is added, its default Design Status is In Design, which
indicates that design is ongoing but is not yet complete.

During the In Design phase, all functionality related to adding and
configuring a Target is available including synchronizing with Map and
using the SQL autogeneration process.

### Design Finished

When a Target is in this Design Status, the design is complete, but the
Target has not gone through the migration process. The Target is locked
down, and no changes are allowed (as in, the Target cannot be edited or
deleted). A Target can only move to this status if it is in sync with
Map. When this Target is synced with Map, {Target Rules} are added.

When a Target in this status is selected, the Sync to Map icon is
enabled.

Updates to Business Contacts and Developers are allowed.

Autogeneration in Data Services and in SQL is allowed.

### Inactive

A Target in this status cannot be edited when:

  - A Target is moved to an Inactive status:
  - The Target is not pushed to Map for mapping and is not available in
    Transform when the Sync to Map process runs.
  - The Target is no longer visible in Map and Construct.
  - Mappings for the Target that are waiting for approval on the Mapping
    Approval page are removed from the page

When a Target in this status is selected, the Sync to Map icon is
disabled.

<span style="font-weight: bold;">NOTE</span>: When a Target is made
inactive, it does not display in Transform.

### Complete

When a Target is in this status, the design is locked down, and no
changes are allowed. A Target can only move to this status if it is in
sync with Map. Auto-generation in Data Services and in SQL is not
allowed.

**NOTE**:When a Target in this status is selected, the Sync to Map icon
is disabled.

Updates to Business Contacts and Developers are allowed.
