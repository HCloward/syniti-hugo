+++
title = 'Activate Fields for Mapping'
solution = 'Migration'
+++

# Activate Fields for Mapping

Activate fields for the Target that are in scope for mapping.
 Deactivate fields if the field should not be mapped.

**NOTE**: Fields can only be activated for a table if the table’s Design
Status is In Design. Target fields cannot be activated or deactivated if
the Target's Design Status is Design Finished, Complete or Inactive.

For a Target field to be mapped in Map on the Field Mappings  page, the
field must be active and visible Refer to [Set Field Visibility for
Mapping](Set_Field_Visibility_for_Mapping) for more information.
Utility field does not exist in the Target system, but is used to
register rules and reports to in Transform.

When adding a field manually, the field is active by default.

When importing fields via a System Type import, all fields are
configured as Inactive unless they are marked for active in the System
Type. An inactive field is one that is not used by the Target system.

If the original mapping action for a Target field created a rule in
Transform, what happens to that rule when the field is deactivated is
determined by a parameter set in Console on the Map tab of the
*Parameters* page. In the Reset Transform Rule list box, the following
options are available:

  - **Delete Transform Rule** – The rule that was created and registered
    in Transform is deleted when the field is deactivated.
  - **Deactivate Transform Rule** – The status of the rule that was
    created and registered in Transform is changed to Inactive in
    Transform when the field is deactivated.
  - **Ignore Transform Rule** – The rule that was created and registered
    in Transform is not affected by the field deactivation.

**NOTE**: A System Type can be configured to automatically activate
certain fields when Target fields are added to a Target via a System
Type import. When the Active For Mapping Default check box is checked
for a field in Common \> System Types \> Tables \> Fields \> Vertical
View, the ACTIVE check box on the Target Fields page is automatically
enabled for the field in Target Design.  Refer to [Add Fields to
Tables](../../../Platform/Common/Use_Cases/Add_Fields_to_Tables) in
Common for more information.

When a field is activated, Map checks the mapping history for that field
to determine whether the field was a previously active field that had
been made inactive. If this is the case, and the field mapping had a
mapping status of Complete when made inactive, Map deletes the field
mapping but the mapping history retains the mapping details. When this
field is again made active, the details of the mapping are retrieved
from the mapping history and used again for the active field mapping.
The mapping status is set to Pending Review. For example, a field
mapping uses a Copy action has the Source table and field to be copied
into the Target field defined and has a mapping status of Complete. A
user selects this field mapping on the Target Fields page in Target
Design and clicks the Deactivate icon in the Page toolbar. The field
mapping is deleted, but the details of the field mapping are retained in
mapping history. A user makes the field active again on the *[Target
Fields](../Page_Desc/Target_Fields_H_Target_Design)* page in Target
Design. The mapping displays on the Field Mappings page in Map with the
details from mapping history (the copy action and the Source table and
Source field to be mapped to the Target field). The mapping status is
set to Pending Review.

If a field is a key field and has the KEY FIELD check box enabled on the
*Target Fields* page, the field cannot be deactivated. Uncheck the KEY
FIELD check box before deactivating the field.

To activate or deactivate a field in Target Design:

1.  Select **Design**  from the Context bar.

2.  Click the **Targets** icon on the
    *[Design](../Page_Desc/Design)* page.

3.  Click the **Fields** icon for a Target.

4.  Select a field.

5.  Click the **ACTIVE** check box to check it.
    
    OR
    
    Click the **ACTIVE** check box to uncheck it.

To activate or deactivate multiple records in Target Design:

1.  Select a contiguous range of records by holding down the **Shift**
    key and selecting the first and last records in the range.
    
    OR
    
    Select a non-contiguous range of records by holding down the
    **Ctrl** key and selecting each record.

2.  Click the **Activate** icon or the **Deactivate** icon in the Page
    toolbar.
