+++
title = 'Create and Approve All Rules'
solution = 'Migration'
+++

# Create and Approve All Rules

The Mapping Approval process is separate from SQL AutoGen. These two
features function independently.

When a user submits a rule in Map:

  - The rule displays on the *[Automation SQL Field
    Mappings](../Page_Desc/Automation_SQL_Field_Mappings_H)* page
    and can be built.
    
    <span style="font-weight: bold;">NOTE:</span> A Rule Where Clause
    can be added on the<span style="font-style: italic;"> [Field
    Mappings](../../Map/Page_Desc/Field_Mappings_H)</span> page’s
    vertical view to filter the records to which a rule is applied.

  - The mapping displays on the *[Mapping
    Approval](../../Map/Page_Desc/Mapping_Approval_H)* page to be
    reviewed by the developer.

If a developer rejects the rule, it is removed from the *[Automation SQL
Field
Mappings](../Page_Desc/Automation_SQL_Field_Mappings_H#Automation_SQL_Field_Mappings_V)*
page and the mapping is reset in Map.

A user can create and approve all rules for an object if there are
multiple mappings.

<span style="font-weight: bold;">NOTE:</span> The target’s Design Status
must be In Design or Design Finished to perform this task.

To approve all rules in AutoGen:

1.  Click the **Automation** tab on the Quick Panel.
2.  Select the Object.
3.  Click the **Create and Approve All Rules** icon in the Page toolbar.

All rules are created for all sources that are registered for the
target.
