+++
title = 'Modify Configuration of Data Source Table Columns'
solution = 'Platform'
+++

# Modify Configuration of Data Source Table Columns

Data Source tables can either be modified or directly added or deleted
from Collect.

To modify the configuration of data source table columns:

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

8.  Click <span style="font-weight: bold;">Column Count</span> for a
    data source table.

9.  Click <span style="font-weight: bold;">Edit</span> for a column to
    modify the data source table column.
    
    Or
    
    Click <span style="font-weight: bold;">Add</span> to add a new
    column to the data source table.
    
    [View the field descriptions for the Data Source Table Columns
    page’s Vertical
    View](../Page_Desc/Data_Source_Table_Columns_H.htm#Data_Source_Table1)

10. Enter column name converted to the defined data type and loaded into
    the target table in <span style="font-weight: bold;">Column</span>
    field.

11. Enter the data type of the source column in
    <span style="font-weight: bold;">From Data Type</span> field.

12. Enter the data length of the source column in
    <span style="font-weight: bold;">From Data Length</span> field.

13. Enter the data precision (total number of digits) of the source
    column in <span style="font-weight: bold;">From Data
    Precision</span> field.

14. Enter the data scale (number of digits after the decimal point) of
    the source column in <span style="font-weight: bold;">From Data
    Scale</span> field.

15. Enter the nullable flag of the source column in
    <span style="font-weight: bold;">From Nullable</span> field.

16. Enter the data type to create tables in the database in
    <span style="font-weight: bold;">Table Create Data Type</span>
    field.

17. Enter the data type of the target column in
    <span style="font-weight: bold;">To Data Type</span> field.

18. Enter the data length of the target column in
    <span style="font-weight: bold;">To Data Length</span> field.

19. Enter the data precision (total number of digits) of the target
    column in <span style="font-weight: bold;">To Data Precision</span>
    field.

20. Enter the data scale (number of digits after the decimal point) of
    the target column in <span style="font-weight: bold;">To Data
    Scale</span> field.

21. Enter the nullable flag of the target column in
    <span style="font-weight: bold;">To Nullable</span> field.

22. Enter the source system SQL function or command to download data
    from the source in <span style="font-weight: bold;">Column
    Override</span> field.
    
    **NOTE:** The <span style="font-weight: bold;">Column
    Override</span> field allows for source system function commands to
    be overridden when data is loaded into the target SQL server tables,
    for example, TO\_CHAR(ORDER\_TIMESTAMP,’YYYYMMDD’) as
    Order\_Timestamp.

23. Click <span style="font-weight: bold;">Save</span>.
