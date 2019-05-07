+++
title = 'Add Fields to Tables'
solution = 'Platform'
+++

# Add Fields to Tables

Once system tables are added, configure fields for the table.

A user can set a static value for the field as well. Refer to [Set
Values for System Types Table
Fields](Set%20Values%20for%20System%20Types%20Table%20Fields.htm) for
more information.

To add fields to tables:

1.  Click **Common \> System Types** in *Navigation* pane.

2.  Click **Tables** icon for System Type.

3.  Click **Fields** icon for Table Name.

4.  Click **Add.**
    
    [View the field descriptions for the System Types Table Fields
    page](../Page_Desc/System_Types_Table_Fields_H.htm)

5.  Enter a unique display order of fields in system table in **FIELD
    ORDER** field.
    
    <span style="font-weight: bold;">NOTE:</span> The display order
    cannot exceed 1600.

6.  Enter a unique name of field in **FIELD** field.
    
    <span style="font-weight: bold;">NOTE:</span> There cannot be
    multiple fields of the same name assigned to a table. The validation
    will fail if the field name is not unique.

7.  Enter a brief description of field in **DESCRIPTION** field.

8.  Click **KEY FIELD** check box to enable it, indicating the field is
    the primary key on the table.

9.  Enter data type of field in **DATA TYPE** field.

10. Enter the number of characters permitted by the field in **LENGTH**
    field.
    
    <span style="font-weight: bold;">NOTE:</span> Enter 0 if the length
    is greater than 4000 characters.

11. Click **Save<span style="font-weight: normal;">.</span>**

12. Click **Vertical View** icon for field to further configure table
    field.

13. Click **Edit<span style="font-weight: normal;">.</span>**
    
    [View the field descriptions for the System Types Table Fields
    page](../Page_Desc/System_Types_Table_Fields_H.htm)

14. Enter SAP help text from the corresponding SAP screen in **Help
    Text** field.

15. Enter number of decimal places allowed by field in **Decimals**
    field.

16. Click **Active For Mapping Default** check box to enable it,
    indicating table field will default to require a mapping action (as
    in, ACTIVE is enabled for a field on the
    <span style="font-style: italic;">Target Fields</span> page in Map).
    The field automatically displays on the
    <span style="font-style: italic;">Field Mappings</span> in Map.
    
    <span style="font-weight: bold;">NOTE:</span> Active For Mapping
    Default is automatically enabled for manually entered fields. This
    check box must be manually checked for system-imported fields.

17. Click <span style="font-weight: bold;">Rule Field</span> check box
    to enable it, marking the field as Rule Only (if
    applicable).
    
    <span style="color: rgb(51, 51, 51);font-family: Arial, sans-serif;line-height: 20px;orphans: auto;widows: auto;-webkit-text-stroke-width: 0px;background-color: #ffffff;display: inline !important;float: none;font-weight: bold;">NOTE:</span>A
    Rule Only field is part of the table creation process, but is
    excluded from being moved between the Source Table to the Source
    Table in the Object database, or between the Source Table in the
    Object database to the Target Table in the Object database.

18. Click **Save.**
