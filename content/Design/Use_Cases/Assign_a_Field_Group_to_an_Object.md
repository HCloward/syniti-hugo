+++
title = 'Assign a Field Group to an Object'
solution = 'Migration'
+++

# Assign a Field Group to an Object

Once a field group has been created, it can be assigned to an Object.
The field group can then be assigned to Target fields for Targets
registered to the Object.

Refer to [Create Field Groups](Create_Field_Groups.htm) for more
information.

To assign a field group to an Object in Target Design:

1.  Select **Configuration \> Field Group Setup** in the *Navigation*
    pane.

2.  Click **Add**.
    
    *[View the field descriptions for the Object Field Groups
    page](../Page_Desc/Object_Field_Groups.htm)*

3.  Select an Object in the **OBJECT ID** list box.
    
    **NOTE**: All Objects in context selected in the Context bar
    display. An Object can have multiple field groups assigned.

4.  Select a field group from the **FIELD GROUP ID** list box.
    
    **NOTE**: Field groups are added on the Field Groups page. Click the
    **+** icon to add a field group. Refer to [Create Field
    Groups](Create_Field_Groups.htm) for more information.

5.  Enter a value the **RULE PRIORITY OFFSET** field.
    
    **NOTE**: If this field is blank when the record is saved, the
    default value -1 is added to the field.
    
    **NOTE**: This number (always negative) is subtracted from the
    rule’s priority to set the order the rule is run. Refer to [Set
    Rule Priority for Fields in Field
    Groups](Set_Rule_Priority_for_Fields_in_Field_Groups.htm) for more
    information.

6.  Click **Save**.
