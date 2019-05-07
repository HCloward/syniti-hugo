+++
title = 'View Configuration of Data Source Table SQL Commands'
solution = 'Platform'
+++

# View Configuration of Data Source Table SQL Commands

Data Source tables SQL commands can be viewed from Collect. The SQL
commands run when the table is created on a build or a download process.
 If there are issues creating a table during the build or download
process, the SQL code from the Data Source Table Create Download SQL can
be copied and run on the target database or source database to create
the table.

To view the configuration of data source table SQL commands:

1.  Click <span style="font-weight: bold;">Targets</span> on the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    target.

3.  Click the <span style="font-weight: bold;">Schedule Groups</span>
    icon for a source.

4.  Click the <span style="font-weight: bold;">Tables</span> icon for a
    schedule group.

5.  Click <span style="font-weight: bold;">Vertical View</span> for a
    table.

6.  Click the <span style="font-weight: bold;">General
    Information</span> tab.

7.  Click <span style="font-weight: bold;">View Design</span>.

8.  Click the <span style="font-weight: bold;">SQL Command</span> icon
    for a data source table.
    
    *[View the field descriptions for the Data Source Table Create
    Download SQL
    page](../Page_Desc/Data_Source_Table_Create_Download_SQL_H.htm)*

The SQL commands are deleted and rebuilt via the BUILD Package process.
They cannot be changed by the user on this page.  Primary Keys and
Indexes are changed via the Index image on the Table. Refer to [Create
Indices for
Tables](Add_Rules_and_Indices_to_Tables.htm#Create_Indices_for_Tables)
for more information. Columns used to create tables and download SQL are
configured under View Design \> Column Count. Refer to [Modify
Configuration of Data Source Table
Columns](Modify_Configuration_of_Data_Source_Table_Columns.htm) for more
information.
