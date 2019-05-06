# Value Map Target Fields from Multiple Source Systems

Map allows value mapping for Target fields that will contain data from
multiple Source systems, such as Oracle, JDE, or some other legacy
system. The values from these Source system fields will be value mapped
to the Target field on the *[Value Mapping (Legacy to
Target)](../Page_Desc/Value_Mapping_Legacy_to_Target_H.htm)* page. Refer
to <span style="color: #0000ff;">[Perform Value
Mapping](Perform_Value_Mapping.htm)</span> for more information. 

Define the Source table and the Source fields from the legacy systems to
add them to the check table that allows them to be value mapped.

**NOTE:** The table and field must exist in a Source database that was
added to a Source in the current context.

To define fields in Map:

1.  Click **Map** in the Context bar.

2.  Click the **Value Mapping** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch_map.htm)* page.

3.  Click the **Mappings** icon for a check table.

4.  Click the check table name link in the **LOOKUP** column on the
    *[Field Mappings](../Page_Desc/Field_Mappings_H.htm)* page next to a
    mapping with Xref or RuleXref action.

5.  Click the **Sources** icon.

6.  Click the **Source Config** icon for a Source and check table
    combination.

7.  Click the **Tables** icon for a Source.

8.  Click **Add**.
    
    <span style="color: #0000ff;">[View the field descriptions for the
    Legacy Value (Source Table Fields)
    page](../Page_Desc/Legacy_Value_Source_Table_Fields_H.htm)</span>

9.  Enter the table name that stores the field in the **SOURCE TABLE**
    field.
    
    **NOTE:** This table must exist in the Source data source that was
    assigned to Wave and Process Area in Console on the *Vertical* View
    of the *[Wave : Process
    Areas](../../Console/Page_Desc/Wave_Process_Areas.htm)* page.

10. Enter the field name in the **SOURCE FIELD** field.
    
    **NOTE:** This field must exist in the **SOURCE TABLE**. 

11. Select an option from the **STATUS** list box.
    
    **NOTE:** If this field is to be value mapped to a Target field,
    select Active for value mapping.

12. Enter the table name that contains the description fields for the
    **SOURCE FIELD** in the **LEGACY DESCRIPTION TABLE** field.

13. Enter the field name that contains the description of the **SOURCE
    FIELD** in the **LEGACY DESCRIPTION** field.

14. Click **Save**.

15. Click the **Refresh** icon for the Check Table to refresh the Source
    legacy values so that they can be value mapped.

16. Click the **Value Mappings** icon for the field to value map these
    newly added Source fields to Target fields.

**NOTE:** After defining the field, click the **View Values** icon to
view all of the values stored in this field that must be value mapped
and the number of records that store each value in the field. The
*[Legacy Value (Source Table
Fields](../Page_Desc/Legacy_Value_Source_Table_Fields_H.htm))* page that
displays also lists the number of records that contain no data for this
field.

**NOTE:** If the remaining values in the Source field should not be
mapped to the Target field click **Remove Values.** This feature removes
all values in the Source field (stored in the Source data source) that
have not yet been value mapped to a Target table.
