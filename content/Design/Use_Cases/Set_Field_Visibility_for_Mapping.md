+++
title = 'Set Field Visibility for Mapping'
solution = 'Migration'
+++

# Set Field Visibility for Mapping

A Migration Developer can set visibility for a field on the
<span style="font-style: italic;">[Target
Fields](../Page_Desc/Target_Fields_H_Target_Design.htm)</span> page.
Visibility determines whether fields display on the
<span style="font-style: italic;">[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H.htm)</span> page in Map
and can be mapped as Source fields, Target fields, or as both Target and
Source fields. Visibility can also be set to None - No mapping required
for the field, indicating that the field does not display on the
<span style="font-style: italic;">Field Mappings</span> page and is not
mapped.

Visibility is useful in cases where fields must have Target Rules built
but must not be Source mapped. For example, if a field always defaults
to the same value, there is no need for mappers to spend time reviewing
the field. The visibility is set to Target – Target only mapping and the
rules are built, but the field does not display on the
<span style="font-style: italic;">Field Mappings</span> page.

In another case, a field’s visibility can be set to Source – Map Source
only. The field is Source mapped, but is not included in Target Rules,
so that metrics accurately reflect mappings status.

<span style="font-weight: bold;">NOTE</span>: Visibility can only be set
if the field’s Target is in a Design Status of In Design.

<span style="font-weight: bold;">NOTE</span>: If the field is Natural,
the visibility is set to Both – Mapping for Source and Target by
default. If the field is a key zLegacy field, the visibility is set to
Source – Source only mapping by default. If the zLegacy field is not a
key field, the visibility is set to None - No mapping required for the
field by default.

The visibility for Utility fields can also be set for columns that are
appended to Target or Source tables. Refer to [Allow Mapping of Utility
Columns](Allow_Mapping_of_Utility_Columns.htm) for more information.

To set visibility for a field in Target Design:

1.  Click <span style="font-weight: bold;">Design</span> in the Context
    bar.

2.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Design](../Page_Desc/Design.htm)* page.

3.  Click the <span style="font-weight: bold;">Fields</span> icon for a
    Target.

4.  Click the <span style="font-weight: bold;">Vertical View</span> icon
    for a field.

5.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Target Fields
    page](../Page_Desc/Target_Fields_H_Target_Design.htm)

6.  Select an option in the
    <span style="font-weight: bold;">Visibility</span> list box.
    
    <span style="font-weight: bold;">NOTE</span>: Values are:
    
      - **Both** – Mapping for Source and Target
      - **None** – No mapping required for the field
      - **Source** – Source only mapping
      - **Target** – Target only mapping

7.  Click <span style="font-weight: bold;">Save</span>.
