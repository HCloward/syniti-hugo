+++
title = 'Activate and Deactivate Tables'
solution = 'Platform'
+++

# Activate and Deactivate Tables

When an Administrator registers a data source in System Administration,
it is automatically registered in Common to be profiled. At this point,
a snapshot of the database is taken and profiling begins.

Tables that are to be excluded from the profile process must be manually
deactivated.

To deactivate/activate tables for profiling:

1.  Click **Common \>  Analyze** in the *Navigation* pane.
    
    **NOTE**: The [Analyze](../Page_Desc/Analyze.htm) page displays Data
    Sources registered in System Administration that are not added to
    the [Ignore Data Sources](Ignore_Data_Sources.htm) page and to which
    the logged in user has security to view. Data Sources are analyzed
    for database object changes, table statistics and duplicate records.

2.  Click **Profile** for Data Source ID.

3.  Click **Tables**.
    
    [View the field descriptions for the Table (Results)
    page](../Page_Desc/Table_Results_H.htm)

4.  Click **Active** check box for a table to disable the check box,
    which excludes the table from being profiled. The Active All Tables
    icon is disabled if all tables are Active.

5.  Click **Inactivate** All Tables on Page toolbar to exclude all
    tables from being profiled and manually activate the select few
    tables to include in profiling. This icon is disabled if all tables
    are Disabled.
