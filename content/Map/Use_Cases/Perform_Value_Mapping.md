+++
title = 'Perform Value Mapping'
solution = 'Migration'
+++

# Perform Value Mapping

On the *Value Mapping (Legacy to Target)* page, where value mapping is
performed, the legacy value and legacy description display. These values
come from the Source check table. During value mapping, select a Target
value or indicate that a legacy value is not relevant for every legacy
value in the check table so that gate metrics can count the value
mapping as complete. 

Besides updating value mappings in the UI as described in this topic, a
user can also:

  - Perform value mapping automatically, if the Source system and Target
    system are identical. On the *Value Mapping* page, click **Auto Map
    By Description** or **Auto Map By Value** in the Page toolbar.

  - Use Excel Integration to download a spreadsheet that users can
    update with value mapping values. Ensure Bulk Execution is enabled
    on the *Value Mapping (Legacy to Target)* page. Once data entry is
    complete, import that data into the DSP. Refer to [Use Excel
    Integration](../../../Platform/Excel_Int/Use_Excel_Integration)
    for more information.

<span style="font-weight: bold;">NOTE:</span> The Source table and
Source field for the check table for the Rule Xref action is not
automatically set. They must be entered on the Vertical View of the
Legacy Value (Source Table Fields) page.

The *[Value Mapping (Legacy to
Target)](../Page_Desc/Value_Mapping_Legacy_to_Target_H)* page
displays all values that are mapped to the Target table in a lookup
table for all Sources.

**NOTE:** A user can update the lookup table configuration in Target
Design by clicking the Target Lookup Table Config icon on the Page
toolbar.

To perform value mapping in Map:

1.  Create a rule with an XRef or RuleXref action on the *[Field
    Mappings](../Page_Desc/Field_Mappings_H)* page. Refer to
    <span style="font-size: 11.0pt;font-family: Arial, sans-serif;color: #0000ff;">[Xref](Xref)</span>
    or
    <span style="font-size: 11.0pt;font-family: Arial, sans-serif;color: #0000ff;">[Rule
    Xref](Rule_Xref)</span> for more information.

2.  Click the **Value Mappings** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch_map)* page.
    
    **NOTE:** The *Value Mapping* page provides an overview of value
    mappings by check table.

3.  Click the **Values** icon for a check table to map all values for
    the selected check table.
    
    **NOTE:** Only those values that are mapped to a Target table
    display. Unmapped values are deleted when the Target is processed.:
    
    **NOTE:** Only those lookup tables with a Type of Configuration are
    available to be value mapped using this process. This value is set
    in Target Design on the *[Target Lookup
    Table](../../Design/Page_Desc/Target_Lookup_Table_H)* page.

4.  Click **Edit**.
    
    *[View the field descriptions for the Value Mapping (Legacy to
    Target) page](../Page_Desc/Value_Mapping_Legacy_to_Target_H)*

5.  Select an option from the **TARGET VALUE** list box
    
    Or
    
    Click the **NOT RELEVANT** check box to check it.

6.   Enter a value that could be used for value mapping in the
    **PROPOSED VALUE** field if applicable.
    
    **NOTE:** The PROPOSED VALUE field is for informational purposes
    only. The count of proposed values displays on the *[Value
    Mapping](../Page_Desc/Value_Mapping)* page.

7.  Enter text in the **COMMENT** field.

8.  Click **Save**.
