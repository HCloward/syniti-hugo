# Add a System Type Model

A System Type Model contains the definition of a system, including the
system’s tables, fields, properties, descriptions and relationships. The
System Type Model can be used to build a complete System Type.

Refer to [System Types](System_Types_Overview.htm) for more information.

A System Type Model is built by creating views that match the required
formats as defined in the system’s data dictionary. Specifically, Model
Views are simple SQL Views that can be written against any system’s data
dictionary to provide all metadata required to build an accurate System
Type. Each Model View has a specific set of required fields and data
types that must be included for the System Type Model to work correctly.

The Model Views are then registered to the System Type Model. Using this
method, a System Type Model can be created for any system.

For an accurate description of the System Type, a System Type Model must
include at least the Table and Table Field Model Views.

To view the required fields and data type formats for a Model View,
click the button next to the Model View on the *[System Types
Models](../Page_Desc/System_Types_Models_H.htm)* page.

A complete System Type Model for SAP and a simplified Model for JDE are
delivered with the DSP®.

An Administrator can add a custom System Type Model.

To add a System Type Model:

1.  Select **Configuration \> System Type Models** in the *Navigation*
    pane.

2.  Click **Add**.
    
    *[View the field descriptions for the System Types Models
    page](../Page_Desc/System_Types_Models_H.htm)*

3.  Enter text in the **SYSTEM TYPE MODEL** text box.

4.  Click **Save**.
