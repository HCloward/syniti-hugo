+++
title = 'Add a Lookup Table Manually'
solution = 'Platform'
+++

# Add a Lookup Table Manually

Lookup tables are a type of table that contains lookup values for
another table. They must be manually added to System Types for systems
where there is not a complete model set up or where the System Types are
manually built.

To add lookup tables:

1.  Click **Common \> System Types** in *Navigation* pane.

2.  Click **Tables** icon for System Type.

3.  Click **Add**.
    
    *[View the field descriptions for the System Types Tables
    page](../Page_Desc/System_Types_Tables_H.htm)*

4.  Enter a lookup table name in the **TABLE NAME** field.

5.  Click **Save**.

6.  Click the **Fields** icon for the newly added table.

7.  Click **Add**.
    
    [View the field descriptions for the System Types Table Fields
    page](../Page_Desc/System_Types_Table_Fields_H.htm)

8.  Enter all fields for the table. Refer to [Add Fields to
    Tables](Add_Fields_to_Tables.htm) for more information.

9.  Once all fields are added, click **Vertical View** for the table on
    the *[System Types Tables](../Page_Desc/System_Types_Tables_H.htm)*
    page.

10. Click **Edit**.
    
    *[View the field descriptions for the System Types Tables
    page](../Page_Desc/System_Types_Tables_H.htm)*

11. Select the description table from **Description Table** list box.
    
    **NOTE:** The description table contains user-friendly descriptions
    of field names.
    
    **NOTE**: This table must already be loaded into System Types.

12. Select description field from **Description Table Field** list box.
    
    **NOTE:** This field contains the user-friendly descriptions for the
    fields on the table.
    
    **NOTE:** The Description Table Field list box values are generated
    from the tables present in the System Type.

13. Select the key field for the description table from **Description
    Table Key Field** list box.

14. Select client field from **Description Table Client Field** list
    box.
    
    **NOTE:** This field is used for SAP only.

15. Select language field from **Description Table Language Field** list
    box.
    
    **NOTE:** This field is used for SAP only.

16. Select a column name from **Lookup Table Field 1** list box to
    specify column name of lookup table.
    
    **NOTE:** The Lookup Table Field 1 list box values are generated
    from the tables present in the System Type.

17. Select additional column name within the lookup table from **Lookup
    Table Field 2 – 5** list boxes to specify column names of the lookup
    table.
    
    **NOTE:** The Lookup Table Field 2-5 list box values are generated
    from the tables present in the System Type.
    
    **NOTE:** The additional lookup table field IDs are used for complex
    lookup tables. Refer to [Set up a Complex Lookup
    Table](../../../Migration/Design/Use_Cases/Set_up_a_Complex_Lookup_Table.htm)
    for more information.

18. Select a column name from **Lookup Table Field Value** list box to
    specify column name of the lookup table. This will default to the
    last column entered.

19. Select a column name from **Lookup Table Client Field** list box to
    specify column name of client column table.
    
    **NOTE:** This field is used for SAP only.

20. Select a column name from **Lookup Table Language Field ID** list
    box to specify column name of language column table.
    
    **NOTE:** This field is used for SAP only.

21. Enter filter to be used when accessing the lookup table in **Where
    Clause** field.

22. Click **Save**.

23. On the [*System Types Tables
    Horizontal*](../Page_Desc/System_Types_Tables_H.htm) View, click the
    **Fields** icon.

24. Click **Edit** for a field on the [*System Types Table
    Fields*](../Page_Desc/System_Types_Table_Fields_H.htm) page.

The lookup table displays as an option in the LOOKUP TABLE list box and
can be added to any field on the table.
