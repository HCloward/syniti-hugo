+++
title = 'Register and Use Sources'
solution = 'Platform'
+++

# Register and Use Sources

A *Source* is a legacy system from where a copy of data is downloaded
and stored in Collect.

Registering and using Sources includes the following actions:

  - [Register Sources to Target](#Register_Sources_to_Target)
  - [Configure Source for SAP Data
    Services](#Configure_Source_for_SAP_Data_Services)
  - [Test Source Connection](#Test_Source_Connection)
  - [Register Tables](#Register_Tables)
  - [Build Package for Source](#Build_Package_for_Source)
  - [View Source Table Metrics](#View_Source_Table_Metrics)
  - [View Summary of Source
Metrics](#View_Summary_of_Source_Metrics)

## <span id="Register_Sources_to_Target"></span>Register Sources to Target

Data can be pulled from multiple sources to a single target; therefore,
multiple sources can be registered to a Target.

To register a source to a target: 

1.  Click **Targets** in *Navigation* pane.

2.  Click **Sources** for Target.

3.  Click **Add**.
    
    [View the field descriptions for the Target Sources
    page](../Page_Desc/Target_Sources_H_Collect)

4.  Select a database name from **SOURCE** list box. The source database
    must be different from the target database.

5.  Update **CONNECTION TYPE** list box if the default value is not
    applicable.
    
    **NOTE:** The CONNECTION TYPE is a valid database connection type
    from source to target.

6.  Select a System Type from **SYSTEM TYPE ID** list box if importing
    group tables from a System Type delivered with Common.
    
    <span style="font-weight: bold;">NOTE</span>: Click the + icon to
    open the System Types page in Common in a new tab to add a System
    Type, if needed.

7.  Update **SCHEMA OWNER** field if the default value is not
    applicable.
    
    **NOTE:** The SCHEMA OWNER controls the schema of the source
    database that contains the tables. The Schema Owner for a source
    cannot be the same as the Schema Owner for an associated target.

8.  Click **Save**; the *Vertical* View displays.
    
    [View the field descriptions for the Target Sources page's Vertical
    View](../Page_Desc/Target_Sources_H_Collect)

9.  Enter a brief description of the Source in **Description** field,
    e.g., DBA or Business Contact information.

10. Click **Advanced Settings** tab.

11. Enter table name of renamed table in target database in **Rename
    Table Template field**, if tables must be renamed when copied to the
    target.
    
    **NOTE:** The **Rename Table Template** field allows the user to
    rename a table in the target database when the target is refreshed
    with source data. The field must contain the value \<TableName\> and
    any prefix or suffix can be used. When the table is downloaded from
    the source, \<TableName\> is replaced with the Rename Table Template
    value. If the table has been previously created, enable **Delete
    Target Table On Build** to recreate the table using the new name.

12. Update **Schedule ID** list box if the default value is not
    applicable.
    
    **NOTE:** The <span style="font-weight: bold;">Schedule ID</span>
    determines when the refresh process is run. Schedules are created
    and maintained in Common. Refer to [Create
    Schedules](../../Common/Use_Cases/Create_Schedules) for detailed
    information.

13. Click **Download Keys Indices** check box to activate it, allowing
    Collect to download primary key indices from non-SAP source system.
    
    **NOTE:** If Download Keys Indices is enabled, Download SQL
    (Configuration \> Connection Types \> Sources) must be defined for
    the database connection type.

14. Click **Delete Target Table on Build** check box to activate it,
    which deletes all previously downloaded tables (and primary keys and
    indices) and rebuilds the table each time a package is built.
    
    **NOTE:** The Delete Target Table on Build setting ensures the most
    recent table schema is downloaded.

15. Select a database connection type from **Data Services Connection
    Type** list box to connect to the source database if using SAP Data
    Services. Values are:

<!-- end list -->

  - AES15

  - DB2 UDBv8

  - DB2 UDBv9

  - Informix v10

  - Informix v11

  - MySQL v5.0

  - MySQL v5.1

  - ODBC

  - Oracle10g

  - Oracle 11g

  - Oracle9i

  - SQL2000

  - SQL2005

  - SQL2008

**NOTE:** The Data Services Connection Type list box displays Data
Sources supported via the DSP’s integration with Data Services. If the
source connects to SAP Data Services, populate the Connection Settings.
Refer to [Configure Source for SAP Data
Services](#Configure_Source_for_SAP_Data_Services) for detailed
information.

16. Click **Sap Settings** tab if SAP is the target database. If SAP is
    not the target database, these fields can remain blank.
    
    **NOTE:** With the SAP Settings fields populated, Collect recognizes
    that the connecting system is SAP. If the actual value is unknown,
    populate these fields with dummy values for the time being (e.g.,
    “NA”). Be sure to update these values before Go-Live.

17. Enter an ID in **SAP User ID** field.

18. Enter the password that corresponds to the User ID in **SAP
    Password** field.

19. Enter name of client within the SAP instance in **Client**
    field.
    
    <span style="color: rgb(51, 51, 51);font-size: 13.63636302948px;line-height: 18.5818176269531px;orphans: auto;widows: auto;-webkit-text-stroke-width: 0px;display: inline !important;float: none;background-color: #ffffff;font-weight: bold;">NOTE:</span>
    The information in this field is used to filter the data downloaded
    from the source. The filter runs against the MANDT column.

20. Click the **All Clients** check box to activate it, if more than one
    SAP client is required. If enabled, data is downloaded for all
    clients in the SAP instance.

21. Click **Remove Client From Key** check box to activate it, which
    builds the Client field (usually MANDT). This feature can only be
    used if one client is being downloaded (i.e., if **All Clients** is
    disabled).

22. Enter a three-character SAP instance used in the source refresh in
    **Instance** field.

23. Enter the default language in **Language** field, e.g., **E** for
    English.

24. Enter system number used to log into SAP in **SAP System Number**
    field so Pool Table data can be refreshed.

**NOTE**: The information in this field is used to filter the data
downloaded from the source. The filter runs against the MANDT column.

**NOTE:** The SAP System Number is located on *SAP GUI Change Item*
screen in SAP so Pool Table data can be refreshed.

1.  Enter server host name in **SAP Server Host** field.
    
    **NOTE:** SAP Server Host is located on *SAP GUI Change Item* screen
    in SAP.

2.  Expand **SapOptional** label to configure RFC options.
    
    <span style="font-weight: bold;">NOTE:</span> If not using an RFC
    connection, the fields under <span style="font-weight: bold;">Sap
    Optional</span> can remain blank.

3.  Update **RFC Name Space Option** list box if default value is not
    applicable. Values are:
    
    NAMESPACE"
    
    NONNAMESPACE

4.  Enter the server host name in **SAP Msg Server Host** if SAP Load
    Balancing is used to download SAP table via RFC.
    
    **NOTE:** If Load Balancing is not used, enter a single space. SAP
    Msg Server Host is located on the SAP GUI.

5.  Enter logon group name in **SAP Logon Group** if SAP Load Balancing
    is used to download SAP table via RFC.
    
    **NOTE:** If Load Balancing is not used, enter a single space. SAP
    Logon Group is located on the SAP GUI.

6.  Click **Save**.
    
    **NOTE**: If the source database is not SAP, close the *Vertical*
    View and continue with [Test Source
    Connection](#Test_Source_Connection).

7.  Click **Sap Settings** tab to test the SAP connection.

8.  Click **Test Sap Connection** to use the provided User ID and
    Password to verify the login credentials are valid. This process
    does not verify the user has security to the source tables within
    SAP.

Continue with Configure Source for SAP Data
Services.

## <span id="Configure_Source_for_SAP_Data_Services"></span>Configure Source for SAP Data Services

If SAP Data Services are being used, specific connection information
used by SAP Data Services must be configured at the Target Source level.
This connection is then tested to ensure that Data Services can connect
to the Source and Target instances.

To configure a source for SAP Data Services:

1.  Click **Targets** in the *Navigation* pane.

2.  Click the **Sources** icon for the Target.

3.  Click **Vertical View** for the Source.

4.  Click the **Advanced Settings** tab.

5.  Click **Edit**.
    
    *[View the field descriptions for the Target Sources page's Vertical
    View](../Page_Desc/Target_Sources_H_Collect)*

6.  Select the name of the target source repository in the **Data
    Services ID** field.
    
    **NOTE:** If this field is blank, the repository set at the target
    level is used. Consider creating and registering an additional
    repository for separate target sources to minimize the chance of
    overloading the communication between Collect and Data Services.

7.  If using change data capture jobs with DBMoto or Data Services,
    click the **Do Not Delete Data** check box to disable it.
    
    **NOTE:** This check box displays once the Data Services ID field is
    populated.

8.  Select a database connection type from the **Data Services
    Connection Type** list box to connect to the source database if
    using SAP Data Services.
    
    **NOTE:** Refer to SAP documentation for details about the types of
    Data Services connections.
    
    **NOTE:** If the Data Services Connection Type is SAP Application
    for a Target Source, the Test Connection icon is disabled on the
    *Target Sources* page *Horizontal* View for that Target Source.
    Connections to SAP can only be made through Data Services or RFC.

9.  Click **Save**.

10. Click **Connection Settings**.

11. Click **Edit**.
    
    [View the field descriptions for the Target Sources – DataServices
    Connection
    page](../Page_Desc/Target_Sources_Data_Services_Connection)
    
    **NOTE:** The fields available on the *Target-Sources – Data
    Services Connection* page vary based on the Data Services Connection
    Type.
    
    Use the following table to populate the applicable
    fields.
    
    |                 |                                                                                                                                                                                                                                                                                                                   |
    | --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
    | Field           | Description                                                                                                                                                                                                                                                                                                       |
    | Server          | Enter server and instance name of the database to which Data Services will connect when building or executing a package.                                                                                                                                                                                          |
    | User            | Enter user ID used to access the database.                                                                                                                                                                                                                                                                        |
    | Password        | Enter password for user ID to access the database.                                                                                                                                                                                                                                                                |
    | Initial Catalog | Enter the database name used by Data Services to connect to a SQL Server.                                                                                                                                                                                                                                         |
    | Host String     | Enter TNS name or string used to connect to the database using the following format: \<Oracle\_system\>/\<Oracle\_SID\>, where Oracle\_system is the IP or network name of the system where Oracle is running, and Oracle\_SID is the Oracle System identifier that identifies the database on the Oracle system. |
    | Database        | Enter the database name where the source or target tables are stored.                                                                                                                                                                                                                                             |
    | odbcDSN         | Enter ODBC Data Source name used to connect to the database.                                                                                                                                                                                                                                                      |
    

    **NOTE:** Once Data Services settings have been configured for the
    Target and Source, SAP Data Services packages can be registered for
    tables, and packages can be built and refreshed.

12. Click **Save**.

Continue with Test Source Connection.

## <span id="Test_Source_Connection"></span>Test Source Connection

Test the Data Source connection to verify the database User ID and
Password login  credentials are connected to the source database.

**NOTE:** The Test Connection feature does not test the validity of the
SAP login credentials or the DSN connection options.

To test the source database connection in Collect

1.  Click the **Targets** icon in the *Navigation* pane.
2.  Click the **Sources** icon for a Target.
3.  Select the Source.
4.  Click the **Test Connection** icon on the Page toolbar to test the
    connectivity to the source database; a confirmation message
    displays.
5.  Click **OK**.
6.  Click the **Vertical View** icon to review the connection metrics.
      - **Test Connection Status** – Displays status of the last test
        connection.
      - **Test Connection On** – Displays last date time of test
        connection.
7.  Continue with Register Tables.

## <span id="Register_Tables"></span>Register Tables

Once the source is set up, register tables. There are two ways to
register tables to a source:

  - **Import a Group Table** – Used to import System Type tables
    delivered with Common. This method facilitates the process of
    registering tables by importing content delivered with Common into
    Collect.

  - **Manually** – Used if the source is not a System Type delivered
    with Common.

Refer to [Register Tables to Source](Register_Tables_to_Source) for
detailed information about this step.

Continue with Build Package for Source.

## <span id="Build_Package_for_Source"></span>Build Package for Source

Building a package for a source includes all active tables included in
the source.

To build a package for a source:

1.  Verify all tables for the source are active.

2.  Verify a package name is listed for all active tables for the
    source.
    
    **NOTE:** If the package name does not display in the list box,
    confirm that the package has been named following naming
    conventions. Refer to [Create
    Packages](../../Assemble/Create_Packages) for more information.

3.  Click **Targets** in *Navigation* pane.

4.  Click **Source** for Target. 

5.  Select the Source.

6.  Click **Build And Refresh** on Page toolbar for Source to build
    package and download tables from source; a confirmation message
    displays. 

7.  Click **Ok**.

**NOTE:** If the package name already exists for the table record, the
table is refreshed (i.e., data is downloaded from the source database).
If the package for the table does not exist, a package is immediately
scheduled to be built and the table is refreshed. The Refresh icon is
disabled for DBMotoMirror package type because the refresh is run by
DBMoto® instead of Collect.

**NOTE:** To receive a workflow email that a table download has failed
in Collect, a user must be assigned to a security role that has the
Collect WebApp group WorkFlowFailureAll or WorkFlowFaiureByTargetAccess
assigned. Refer to [Set
Security](../../Sys_Admin/Use_Cases/Setting_security) in System
Administration for more information.

Continue with View Source Table Metrics.

## <span id="View_Source_Table_Metrics"></span>View Source Table Metrics

View monthly, weekly and daily metrics for the number of tables
downloaded for a source.

To view sources metrics:

1.  Click **Targets** in *Navigation* pane.
2.  Click **Sources** for Target.
3.  Click **Metrics** for Source.
4.  Click **Metrics** to view monthly, weekly or daily metrics; a graph
    plotting the metrics
display

## <span id="View_Summary_of_Source_Metrics"></span>View Summary of Source Metrics

A series of charts are available that display monthly, weekly and daily
metrics for the Target Source.

To view a summary of source metrics:

1.  Click <span style="font-weight: bold;">Targets</span> in
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Sources</span> for a target.
3.  Click <span style="font-weight: bold;">Metrics</span> for a Target
    Source.

[View the field descriptions for the Target Source Metrics Charts
page](../Page_Desc/Target_Source_Metric_Charts)
