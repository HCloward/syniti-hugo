+++
title = 'Allow Mapping of Utility Columns'
solution = 'Migration'
+++

# Allow Mapping of Utility Columns

A Utility field does not exist in the Target system, but is used to
register rules and reports in Transform. Fields of this type should be
captured in Target Design. A Utility field is added to the Target table
to be used by AutoGen.

Visibility is set to None by default for appended utility columns.
However, the visibility setting can be configured to allow utility
columns to be mapped if needed.

A Migration Developer can set visibility for append utility columns on
the <span style="font-style: italic;">[Append Utility
Columns](../Page_Desc/Append_Utility_Columns)</span> page.
Visibility determines whether fields display on the
<span style="font-style: italic;">[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H)</span> page in Map
and can be mapped as Source fields, Target fields, or as both Target and
Source fields. Visibility can also be set to None, indicating that the
field does not display on the <span style="font-style: italic;">Fields
Mappings</span> page and is not mapped.

Field visibility can also be defined for Target fields. Refer to [Set
Field Visibility for Mapping](Set_Field_Visibility_for_Mapping) for
more information and for general information about the visibility
setting.

Field defined as Append columns can be appended to all Target or Source
tables, depending on how the fields are configured. Refer to [Append
Utility Columns to All Tables](Append_Utility_Columns_to_all_Tables)
for more information.

<span style="font-weight: bold;">NOTE</span>: If a user deletes an
append column, if it has already been synced with Map, the column still
appears on the Target table. To remove the append column in this case,
set the column to inactive.

To set visibility for appended utility columns in Target Design:

1.   Select <span style="font-weight: bold;">Configuration \> Append
    Utility Columns</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Edit</span>.
    
    **NOTE**: The zSource column is installed with the platform and
    cannot be edited or deleted.
    
    [View the field descriptions for the Append Utility Columns
    page](../Page_Desc/Append_Utility_Columns)

3.  Select an option in the
    <span style="font-weight: bold;">VISIBILITY</span> list box.
    
    <span style="font-weight: bold;">NOTE</span>: Values are:
    
      - **Both** – Mapping for Source and Target
    
      - **None** – No mapping required for the field
    
      - **Source** – Source only mapping
    
      - **Target** – Target only mapping

4.  Click <span style="font-weight: bold;">Save</span>.
