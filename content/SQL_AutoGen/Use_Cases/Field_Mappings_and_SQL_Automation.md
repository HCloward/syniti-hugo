+++
title = 'Field Mappings and SQL AutoGen'
solution = 'Migration'
+++

# Field Mappings and SQL AutoGen

After mappings are submitted on the *Field Mappings* page, they are used
as the basis for rule generation.

Records display on the *[Automation SQL Field
Mappings](../Page_Desc/Automation_SQL_Field_Mappings_H)* page after:

  - Target and source have been added and configured in Target Design.
  - Field mappings for the target and source have been submitted in Map.
  - Complex or basic rules have been added to a target field in Target
    Design, if needed.

To view the status of all mappings for the target, click Mappings for an
object on the *[Automation](../Page_Desc/Automation_page)* page to
open the *[Field Mappings](../../Map/Page_Desc/Field_Mappings_H)*
page in Map.

To view mappings that can be used as the basis for generation of rules,
click Mappings Completed for an object on the *Automation* page to open
the *Automation SQL Field Mappings* page. All mappings with a Mapping
Status of Complete display.

**NOTE:** If a mapping has a Mapping Status of Complete, the mapping has
either been:

  - Changed to the status by a mapper when the mapping is complete. The
    status must be Complete before the mapping can be submitted.
  - Set by the platform when the Developer approves the mapping on the
    *Mapping Approval* page.

**NOTE:** If using AutoGen, a user can create and approve all rules at
once. In this case, the Mapping Status is updated to Complete for all
mappings in the selected target. Refer to [Create and Approve All
Rules](Create_and_Approve_all_rule) for more information.

**NOTE:** The Mapping Approval process and the AutoGen process function
independently. AutoGen can take place for mappings that are in a
Complete status but have not yet been approved.

<span style="font-weight: bold;">NOTE:</span> The *Automation SQL Field
Mappings* page displays behind the *Automation* page and, depending on
how the user’s view is configured, may be obstructed by the *Automation*
page itself. In this case, to view the *Automation SQL Field Mappings*
page either close the *Automation* page or reduce the size of the
*Automation* page.
