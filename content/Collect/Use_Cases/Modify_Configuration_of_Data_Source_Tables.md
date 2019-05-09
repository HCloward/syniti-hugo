+++
title = 'Modify Configuration of Data Source Tables'
solution = 'Platform'
+++

# Modify Configuration of Data Source Tables

Collect stores internal configuration data from the source. This
information can be modified to reduce visible columns or to see how the
source was downloaded.

To modify the configuration of source tables:

1.  Click <span style="font-weight: bold;">Targets</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Sources</span> for a target.

3.  Click <span style="font-weight: bold;">Schedule Groups</span> for a
    source.

4.  Click <span style="font-weight: bold;">Tables</span> for a schedule
    group.

5.  Click <span style="font-weight: bold;">Vertical View</span> for a
    table.

6.  Click <span style="font-weight: bold;">General Information</span>
    tab.

7.  Click <span style="font-weight: bold;">View Design</span>.

8.  Click <span style="font-weight: bold;">Edit</span> to modify a data
    source table.
    
    [View the field descriptions for the Data Source Tables
    page](../Page_Desc/Data_Source_Tables_H)

9.  Update the <span style="font-weight: bold;">PACKAGE NAME</span>
    field, if applicable, to modify the name of the package that
    refreshes the target table with source data.
    
    **NOTE:** The package name must follow the naming convention
    \#Database\#%\#Source\#%.  Refer to [Create
    Packages](../../Assemble/Create_Packages) for more information.

10. Click <span style="font-weight: bold;">Save</span>.

11. Click <span style="font-weight: bold;">Vertical View</span>.

12. Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the Data Source Tables page’s
    vertical
    view](../Page_Desc/Data_Source_Tables_H#Data_Source_Tables_V)
    
    **NOTE: **<span style="font-weight: bold;">Table Rename</span>
    field, if applicable, will display the renamed table in the target.
    If table rename needs to be changed, delete the View Design
    record. Update the Table Rename on the
    <span style="font-style: italic;">Vertical</span> view of the Table
    and click Build Package. Table Rename should not be changed on this
    page.

13. Update <span style="font-weight: bold;">Target Time Out</span>
    field, if applicable, to modify the number of seconds the target
    runs before timing out.

14. Update <span style="font-weight: bold;">Source Time Out</span>
    field, if applicable, to modify the number of seconds the source
    runs before timing out.

15. Click <span style="font-weight: bold;">Save</span>.

16. Return to the <span style="font-style: italic;">Horizontal</span>
    View; two icons are available for further data source table
    configuration:

<!-- end list -->

  - Click <span style="font-weight: bold;">Column Count</span> to modify
    columns within the source table. Refer to [Modify Configuration of
    Data Source Table
    Columns](Modify_Configuration_of_Data_Source_Table_Columns) for
    detailed information.
  - Click <span style="font-weight: bold;">SQL Command</span> to view
    the SQL commands used in the download package. Refer to [View
    Configuration of Data Source Table SQL
    Commands](View_Configuration_of_Data_Source_Table_SQL_Commands)
    for more information.
