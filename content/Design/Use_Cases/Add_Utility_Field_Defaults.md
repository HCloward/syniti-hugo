+++
title = 'Add Utility Field Defaults'
solution = 'Migration'
+++

# Add Utility Field Defaults

Utility fields can be appended to all Target and/or Source tables
automatically.

A Utility field does not exist in the Target system, but rules and
reports are registered to it in Transform. Fields of this type should be
captured in Target Design but should not be mapped and will not display
in Map. A Utility field is added to the Target table to be used by
AutoGen.

A Designer can add default values on the *[Utility Field
Defaults](../Page_Desc/Utility_Field_Defaults.htm)* page that can be
selected for a column on the *[Append Utility
Columns](../Page_Desc/Append_Utility_Columns.htm)* page.

<span style="font-weight: bold;">NOTE</span>: Some default values are
added by the system at installation and cannot be edited or deleted.
These values can be used to enable or disable a setting, display the
current date and time, add a unique identifier, or use a static value.

The options added on this page are available to be selected in the
DEFAULT VALUE list box and can be assigned to Utility columns on the
<span style="font-style: italic;">[Append Utility
Columns](../Page_Desc/Append_Utility_Columns.htm)</span> page. Refer to
[Append Utility Columns to All
Tables](Append_Utility_Columns_to_all_Tables.htm) for more information.

To add a default value in Target Design:

1.  Select **Configuration \> Utility Field Defaults** in the
    *Navigation* pane.

2.  Click **Add**.
    
    *[View the field descriptions for the Utility Field Defaults
    page](../Page_Desc/Utility_Field_Defaults.htm)*

3.  Enter a name in the **DEFAULT VALUE** field.
    
    <span style="font-weight: bold;">NOTE</span>: This name displays in
    the **DEFAULT VALUE** list box on the *[Append Utility
    Column](../Page_Desc/Append_Utility_Columns.htm)* page.

4.  Enter a default value in the
    <span style="font-weight: bold;">DEFAULT VALUE</span> field.

5.  Enter a description of the default in the **DESCRIPTION** field.

6.  Click **Save**.
