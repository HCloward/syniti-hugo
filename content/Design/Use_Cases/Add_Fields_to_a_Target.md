# Add Fields to a Target

While the easiest method to add fields to a Target is through import, a
user can also manually add Target fields.

In a typical migration, field data is downloaded from a System Type from
dspCloud and imported into Target Design along with the Target table.

Fields may be manually added in cases where only a few additional fields
are required. Fields added manually are usually Utility fields which do
not exist in the Target system, but are used to register rules and
reports to Transform.

**NOTE**: Many of the fields on the
<span style="font-style: italic;">Target Fields</span> page contain data
after Targets are imported. When manually adding a field, many of these
fields are not required.

<span style="font-weight: bold;">NOTE</span>: The data type of a field
determines whether the Length and Decimal fields, displaying on the
<span style="font-style: italic;">Target Fields</span> page’s
<span style="font-style: italic;">Vertical</span> View, are required.
When the following data types are selected, the Length field is required
to have a value:

  - NVARCHAR
  - DECIMAL
  - NCHAR
  - NVARCHAR

When the DECIMAL or DATETIME data types are selected, the Decimal field
is required to have a value.

<span style="font-weight: bold;">NOTE</span>: If the field is a zLegacy
field:

  - The NAME, KEY and LOOKUP TABLE fields on the
    <span style="font-style: italic;">[Target
    Fields](../Page_Desc/Target_Fields_H_Target_Design.htm)</span> page
    cannot be edited.
  - The Extend to Field Groups option is not available.
  - Basic Rules and Complex Rules cannot be configured.

To add fields to a Target in Target Design:

1.  Select **Design** in the Context bar.

2.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Design](../Page_Desc/Design.htm)* page.

3.  Click the **Fields** icon for a Target.

4.  Click **Add**.
    
    **NOTE**: The Add button does not display on the *Target Fields*
    page until a Target in a Design Status of In Design is selected on
    the *Targets* page. The Add button does not display if the selected
    Target has a Design Status of Design Finished, Complete or Inactive.
    
    *[View the field descriptions for the Target Fields
    page](../Page_Desc/Target_Fields_H_Target_Design.htm)*

5.  Enter a number in the <span style="font-weight: bold;">FIELD
    ORDER</span> field.
    
    **NOTE**: The order is used to sort the
    <span style="text-indent: -60px;font-style: italic;">Field
    Mappings</span><span style="text-indent: -60px;"> page in Map
    (ProcessArea \> Targets \> Mappings). Key and required fields are
    given a lower number (as in, a higher priority) than optional
    fields.</span>

6.  Enter the field name in the **NAME** field.

7.  Enter the name that displays on the application screen in the
    <span style="font-weight: bold;">DISPLAY NAME</span> field, if
    needed.

8.  Select an option in the **LOOKUP TABLE** list box.
    
    **NOTE**: Click the **+** icon to open the *[Target Lookup
    Table](../Page_Desc/Target_Lookup_Table_H.htm)* page to add a lookup
    table if needed. Refer to [Set Up Lookup
    Tables](Set_up_a_Simple_Lookup_Table.htm) for more information.

9.  Select an option in the
    <span style="font-weight: bold;">USAGE</span> field if necessary.
    
    **NOTE**: The option in the USAGE field is inherited from the Target
    level. Values are:
    
      - **Natural** – A field that exists in the Target system.
    
      - **Utility** – A field that does not exist in the Target system,
        but is used to register rules and reports to in Transform.
        Fields of this type should be captured in Target Design but
        should not be mapped and will not display in Map. A utility
        field is added to the Target table to be used by Auto
        Generation.

10. Select the field’s requirement status in the **REQUIRED** list box.
    
    **NOTE**: Values are:
    
      - **Business Required** – Required to meet a business rule or
        otherwise meet a business need.
      - **Technical Required** – Required by the system.
      - **Conditional** – Required depending on certain conditions.
      - **Optional** – Not required.
    
    Values in this list box can be added on the
    <span style="font-style: italic;">Required</span> page
    (Configuration \> Required). Refer to [Add Custom Requirement
    Settings](../Config/Add_Custom_Requirement_Settings.htm) for more
    information.

11. Select an option in the **CRITICALITY** list box.
    
    **NOTE**: This value is used for reporting.
    
    **NOTE**: Custom Criticality values can be added on the
    <span style="font-style: italic;">Criticality</span> page
    (Configuration \> Criticality). Refer to [Add Custom Criticality
    Levels](../Config/Add_Custom_Criticality_Levels.htm) for more
    information.

12. Disable the **ACTIVE** check box if the field should not be mapped
    and should not be included in Auto Generation. Refer to [Activate or
    Deactivate Target Fields for Mapping](Activate_Fields_for_Map.htm)
    for more information.

13. Click the **KEY FIELD** check box if the field is the key on the
    table.
    
    **NOTE**: When a field has the KEY FIELD check box enabled, Design
    creates a zLegacy field that is synced to Map for mapping. A zLegacy
    field can be deleted, except in cases where the field it was created
    for is marked as a Natural Key field. In this case, if the zLegacy
    field is deleted in Target Design, it will be added back when Target
    Design and Map are synced. For example, the MATNR field is a Key
    field and a Natural field for the ttMARA Target table. The
    zLegacyMATNR field is created automatically. A user deletes the
    zLegacy MATNR field, while the MATNR field remains a Natural Key
    field. When a user clicks the Sync to Map icon on the
    *[Targets](../Page_Desc/Targets_H_Design.htm)* page, the zLegacy
    MATNR is added back to the Target.
    
    **NOTE**:Key fields are created during field mapping. Keys on the
    Target table are created by using the key(s) from the Target system
    and the zLegacy field. For example, the MATNR field identified as
    the key field in Target Design is used to create the key field
    zLegacyMATNR on the Target table.

14. Click the **VERIFY POST LOAD** check box to check it if this field
    should be verified after it is loaded into the Target ERP system.
    
    **NOTE**:A process runs after the data is loaded to verify the
    field.

15. Click **Save**.
    
    **NOTE**: Once the Design Status is set to Design Finished or
    Complete, these fields are pushed into Map as Target fields that can
    be mapped on the *[Field
    Mappings](../../Map/Page_Desc/Field_Mappings_H.htm)* page.
