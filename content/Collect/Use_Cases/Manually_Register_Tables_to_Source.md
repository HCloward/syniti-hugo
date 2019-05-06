# Manually Register Tables to Source

To manually register a table to a source:

1.  Click **Targets** in the
    *<span style="font-size: 11.0pt;">Navigation</span>* pane.

2.  Click **Sources** for Target.

3.  Click **Tables** for Source.

4.  Click **Add**.
    
    [View the field descriptions for the Tables
    page](../Page_Desc/Tables_H.htm)

5.  Enter a name in **TABLE** field.

6.  Update **PACKAGE TYPE** list box if the default value is not
    applicable.
    
    **NOTE:** The PACKAGE TYPE controls the method in which target
    tables are refreshed with source data. Refer to [Package
    Types](Package_Types.htm) for detailed information on each supported
    package type.
    
    **NOTE:** Refer to [Use the Manual Data Services Package
    Type](Use_the_Manual_Data_Services_Package_Type.htm) for more
    information about using this package type.

<!-- end list -->

1.  Update **PRIORITY** field if the default value is not applicable.
    
    **NOTE:** The PRIORITY field controls the order in which tables are
    processed.

2.  Verify **ACTIVE** check box is enabled to include the table in a
    source refresh.

3.  Click **Save**.

4.  Click **Vertical View** for a Table.

5.  Click **Edit**.
    
    [View the field descriptions for the Tables page's Vertical
    View](../Page_Desc/Tables_H.htm)

6.  Enter a brief table description in **Description** field.

7.  Click **Advanced Settings** tab.

8.  Enter text in **Table Rename** field if the table needs to be
    renamed in the source database.
    
    **NOTE:** The Table Rename field enables the user to rename a table
    in the target database. The field must contain the value
    \[TableName\]. At run time, this value is replaced by the processing
    table name.

9.  Enter a value in **Where Clause Override** field if data must be
    filtered during a download process.
    
    **NOTE:** The Where Clause Override is an extra clause that
    conditions to the download SQL, e.g., WHERE SPRSL NOT IN
    (‘a’,’b’,’c’,’d’) and Where ColumnKey like ‘2007%’.
    
    **NOTE:** When a Where Clause Override is added to a table that is
    set up as a Data Services package the initial build will require an
    additional build. Immediately after the first build runs, the user
    must rerun the build. The second build will use the clause entered
    in the Where Clause Override field to refresh the table’s contents
    when a refresh is run. After the second build, the clause entered in
    the Where Clause Override field will be up to date for every
    subsequent build, and the user is not required to build the package
    more than once.

10. Enter the database’s schema for the table in **Table Schema Owner**
    field.

11. Select a package from **Package Name** list box.
    
    **NOTE:** If the Package Type is set to **Manual**, the Package Name
    field must be populated. For Manual Data Services package types,
    select from the list of available jobs in the Data Service
    Repository assigned to the target on the
    *[Targets](../Page_Desc/Targets_H_Collect.htm#Targets_V)* page’s
    *Vertical* View.
    
    **NOTE:** If the package name does not display in the list box,
    confirm that the package has been named following naming
    conventions. Refer to [Create
    Packages](../../Assemble/Create_Packages.htm) for more information.

12. Update **Schedule ID** list box if the default value is not
    applicable.
    
    **NOTE:** The <span style="font-weight: bold;">Schedule ID</span>
    determines when the refresh process runs. If a schedule is set at
    the table level, the source schedule for the table is ignored.
    Schedules are created and maintained in Common. Refer to [Create
    Schedules](../../Common/Use_Cases/Create_Schedules.htm) for more
    information.

13. Update **Schedule Group** list box if the default value is not
    applicable.
    
    **NOTE:**   TheSchedule Group field controls the schedule to build
    packages, refresh or filter on tables in a group.

14. Click **Synchronous** check box to allow packages for Data Services
    jobs execute synchronously.
    
    **NOTE:** With synchronous execution, the build package jobs respect
    the queue and wait until jobs are finished before starting another
    job. This option applies to the data services [Package
    Types](Package_Types.htm).

15. Click **Schedule Single Thread** check box if the table is to be
    downloaded in a queue with all other single-threaded tables.
    
    **NOTE:** If **Schedule Single Thread** is enabled, a Schedule Group
    must be assigned in order for tables to be downloaded in a single
    thread. If Schedule Single Thread is disabled, tables are downloaded
    in a logical grouping. Schedule Single Thread is ignored if Package
    Type is “DBMoto to Mirror” or "Data Services." 

16. Update **Rfc Records Per Call** field if the default value is not
    applicable.
    
    **NOTE:** The Rfc Records Per Call only applies to RFC package types
    (BOA RFC, SAP RFC, and SAP TEXT). This field controls the number of
    records returned in a single block for Collect background process to
    parse and insert into the database.

17. Click **Save**.
