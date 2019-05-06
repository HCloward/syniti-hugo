# Add Mappings

Mappings are generic mappings between a source and a target system.
Mapping fields drive the import process in Map. Mapping fields must be
manually added to System Types.

To add mappings:

1.  Click **Common \> System Types** in *Navigation* pane.

2.  Click **TargetMappings** icon for System Type.

3.  Click **Add**.
    
    [View the field descriptions for the System Types Mappings
    page](../Page_Desc/System_Types_Mappings.htm)

4.  Select a table-field combination within the source system being
    mapped from **SOURCE SYSTEM TYPE TABLE ID** combo box.

5.  Enter a brief description of mapping in **DESCRIPTION** field.

6.  Select a table field within the target system being mapped from
    **TARGET SYSTEM TYPE TABLE FIELD ID** list box.

7.  Select option in the a type **ACTION** list box to determine how the
    data in the fields is to be mapped. Values are:
    
      - **Construction** – Constructs data in Construct because source
        data does not exist for this Target ERP field.
      - **Copy** – Copies the legacy value directly into the Target ERP
        system, unchanged.
      - **Cross Reference** – Cross references the legacy value using
        value mapping to convert the source value to a Target ERP value.
      - **Default** – Defaults all records to value in DEFAULT VALUE
        field.
      - **Internal** – Generates number inside Legacy system as the
        record is loaded, which is typically the key value.
      - **Manual Construction** – Indicates a rule that will be built
        manually in Construct
      - **ManualRule** – Creates rule using provided SQL code.
      - **Not Used** – No mapping is required because the field will not
        be loaded into the Target ERP system.
      - **Rule** – Creates a rule for complex field mapping. Any action
        that is too complex for a Default, Copy or Cross Reference.
      - **Rule Cross Reference** – Performs manipulation of the source
        value and then converts the value to a Target ERP value using
        value mapping.

8.  Enter SQL code used to generate the rule in **RULE SQL** list box.

9.  Enter value to be defaulted for all rows in **DEFAULT VALUE** field.
    
    <span style="font-weight: bold;">NOTE</span>: This value is only
    used when the action is Default, and, in this case, is required.

10. Enter additional information about the rule in **RULE COMMENT**
    field.

11. Select a rule type from the **RULE TYPE** list box to determine the
    rule category to import mappings (as in, a source rule or a target
    rule).
    
      - **SourceRule** — The SQL rule is imported as a source rule to be
        run on Target Source data.
      - **TargetRule** — The SQL rule is imported as a target rule to be
        run on target data.
    
    <span style="font-weight: bold;">NOTE</span>: This field is used,
    and required, if the action is Copy, Cross Reference or Rule Cross
    Reference.

12. Enter the source or target rule value used to determine the rule
    category to import mappings in **RULE TYPE** field.

13. Select a group name from **MAPPING GROUP ID** list box.
    
    <span style="font-weight: bold;">NOTE</span>: All mappings belong to
    the default mapping group (\*).

14. Enter a field group name to further categorize the mapping in
    **FIELD GROUP** field.

15. Click **Save**.
