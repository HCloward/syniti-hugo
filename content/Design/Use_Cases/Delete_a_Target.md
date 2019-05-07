+++
title = 'Delete a Target'
solution = 'Migration'
+++

# Delete a Target

Before deleting a Target, be aware of the downstream implications.

<span style="font-weight: bold;">NOTE</span>: Deleting a Target removes
all mappings set for the Target and all settings related to the Target
in Transform. If a mapping associated with the Target is waiting for
approval and the Target is deleted, the mapping is removed from the
Mapping Approval page.

When a Target is deleted in Target Design:

  - Targets are automatically deleted in Map and Transform
  - Basic and complex rules for the Target are also deleted
  - Metrics that use the Target are updated to remove data related to
    the deleted Target
  - Pending approvals for the Target are deleted from the *[Mapping
    Approvals](../../Map/Page_Desc/Mapping_Approval_H.htm)* page
  - Objects that have been built in the database such as tables, views
    and store procedures must be manually  removed
  - Construction tables and views will not be deleted, and the entry
    will still exist in the DCS database; however, the tables will not
    be accessible through Construct
