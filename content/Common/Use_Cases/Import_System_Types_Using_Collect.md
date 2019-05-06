# Import System Types Using Collect

If you do not have access to a System Type model or a data dictionary
for a system, you can use the Fetch and Build and Refresh options in
Collect to import all tables available in a Collect target source into a
System Type.

To import a System Type using Collect:

1.  [Register a Data Source in System
    Administration](../../Sys_Admin/Use_Cases/Register_a_Data_Source.htm).

2.  [Register the source to a Target in
    Collect.](../../Collect/Use_Cases/Register_and_Use_Sources.htm#Register_Sources_to_Target)
    
    **NOTE:** Make sure to select the correct Connection Type, as this
    determines the query used to fetch the target system's table and
    field metadata.
    
    **NOTE:** You can either select an existing System Type to add to or
    click the link to create a new one. You only need to enter a name
    for the System Type.

3.  Click the **Vertical View** icon for the Target Source.

4.  Click the **Action** tab.

5.  Click the **Fetch Tables** icon to retrieve all of the table names
    from the system's metadata and import them into the System Type.
    
    **NOTE:** By default, these tables are added to a group in the
    System Type as inactive in that group. You can check the Activate
    Fetched Tables checkbox on the Action tab to have all of the tables
    in the System Type Group imported as active.

6.  [Activate or Deactivate Tables in the System Type Model Group in
    Common as needed.](ActiveDeactiveTblsSystmTypeModelGrp.htm)
    
    **NOTE:** If you selected the Activate Fetched Tables checkbox in
    Collect, then you must deactivate the tables in the group for which
    you do not want to have field-level metadata.

7.  [Import System Types Group
    Tables.](../../Collect/Use_Cases/Import_Group_Tables.htm)
    
    **NOTE:** After the Import process is complete, click the **Build
    and Refresh** icon. Wait for this process to complete before moving
    on to the final steps in Common.

8.  Select **Common \> System Types** in the *Navigation* pane.

9.  Click the **Vertical View** icon for the System Type.

10. Click the **Import From Data Source or Model** icon in the Page
    toolbar.

11. Click **Edit** on the *[System Types
    Import](../Page_Desc/System_Types_Import.htm)* page.

12. Select the data source of the Collect target to which you registered
    your target source.
    
    **NOTE:** This is a dg% data source for target systems or an sdb%
    data source for source systems.

13. Click **Save**.

14. Click the **Import** icon in the Page toolbar; once the import
    process is complete, your System Type should contain field-level
    metadata for all the tables you built and refreshed from the Collect
    Target Source.

**NOTE:** This method of importing a System Type only imports the tables
and field structures into the System Type. No associated metadata such
as field descriptions, joins, or lookup tables are imported.
