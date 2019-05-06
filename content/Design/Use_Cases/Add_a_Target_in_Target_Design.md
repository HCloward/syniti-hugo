# Add a Target

While the easiest method to add a Target table is through import, a user
can also manually enter a Target, and then manually add fields to it.

Refer to [Import a Target Design from a System
Type](Import_from_a_System_Type.htm), [Import Target Design from a
Database](Import_from_a_Database.htm), [Import Target Design from an
Excel File](Import_from_an_Excel_File.htm), and [Add Fields to a
Target](Add_Fields_to_a_Target.htm) for more information.

To add a Target:

1.  Select **Design \> Targets** in the Context bar.

2.  Click **Add**.

3.  *[View the field descriptions for the Targets
    page](../Page_Desc/Targets_H_Design.htm)*

4.  Select an Object from the **OBJECT ID** list box.
    
    **NOTE**: These Objects were added in Console. The Objects that
    display are associated with the Wave and Process Area selected in
    the Context bar. Refer to [Add an
    Object](../../Console/Use_Cases/Add_Elements_Separately.htm#Add3)
    for more information.

5.  Enter a value in the **PRIORITY** text box.
    
    **NOTE**: PRIORITY is the order of importance in which Targets are
    to be built and mapped.

6.  Enter a name starting with tt in the **NAME** field.
    
    **NOTE**: This table will be created in the Target database and must
    be a unique name. If another Target with this name has already been
    added to this object, an error displays.

7.  Enter a brief description about the Target in the **DESCRIPTION**
    field.
    
    **NOTE**: All Targets are added with the default DESIGN STATUS of In
    Design, which displays as a link in the DESIGN STATUS column.
    Clicking this link does not open the
    <span style="font-style: italic;">[Set Design
    Status](Set_Design_Status.htm)</span> page until the Target is
    saved.

8.  Select an option from the **USAGE** list box.
    
    **NOTE**: Values are:
    
      - <span style="font-weight: bold;">Natural</span> – The field
        exists in the Target system.
      - <span style="font-weight: bold;">Utility</span> – The field does
        not exist in the Target system, but can be used to register
        rules and reports to in Transform. Fields of this type should be
        captured in Target Design. A utility field is added to the
        Target table to be used by the AutoGen process.  Utility fields
        will be appended to BOTH the Target and source table as is.  No
        “z” field will be appended.

9.  Select an option in the **SYSTEM TYPE ID** list box, if necessary.
    
    **NOTE**: If the Target needs to be exported, a System Type must be
    entered.
    
    **NOTE**: These System Types were added in Common. Refer to [Add
    System
    Types](../../../Platform/Common/Use_Cases/Add_System_Types.htm) for
    more information.
    
    **NOTE**: Importing a System Type is the most common method of
    adding a Target. Refer to [Import a Target Design from a System
    Type](Import_from_a_System_Type.htm) for more information.

10. Enter a table name in the **TARGET SYSTEM TABLE NAME** field.
    
    **NOTE**: Enter the same name as the one in the **NAME** field
    without ‘tt’ at the start. For example, if the NAME field contains
    ttKNAI, enter KNAI in the **TARGET SYSTEM TABLE NAME** field.

11. Click **Save**.
