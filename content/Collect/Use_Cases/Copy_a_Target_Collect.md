+++
title = 'Copy a Target'
solution = 'Platform'
+++

# Copy a Target

The Copy Target functionality copies all sources, tables, rules and
indices from the source to the destination target and is primarily used
for server migration. Before a target can be copied, the connection to
the new target databases must first be established in the connection
table and in the data source.

To copy a target:

1.  Establish a connection to the new target database in the connection
    table and in Common. Refer to [Register a Data Source in
    Common](../../Common/Use_Cases/Register_a_Data_Source_in_Common)
    for detailed information.

2.  Select **Tools \> Copy Targets** in the *Navigation* pane.

3.  Click **Edit**.
    
    [View the field descriptions for the Copy Targets
    page](Copy_a_Target_Collect)

4.  Select a database from **Target From** list box, where tables, rules
    and indices are currently configured.

5.  Select a database from **Target To** list box, where tables, rules
    and indices are to be copied.
    
    **NOTE:** Databases for Target From and Target To must be registered
    in Common with a SQL Server DBMS type. Targets cannot be Oracle, DB2
    or other ODBC connections.

6.  Click **Save**.

7.  Click **Copy Target** to copy all sources, both active and inactive,
    (including tables, rules and indices) from the Target From to the
    Target To database – the process only copies records to the target
    database that do not exist; a confirmation message displays.

8.  Click **Ok**.
