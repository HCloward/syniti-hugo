+++
title = 'Register and Use Targets'
solution = 'Platform'
+++

# Register and Use Targets

Targets are destination databases where tables are refreshed with source
data.

Registering and using targets includes the following actions:

  - [Register Targets](#Register_Targets)
  - [Test Target Connection](#Test_Target_Connection)
  - [Assign Target Security](#Assign_Target_Security)
  - [Register Sources](#Register_Sources)
  - [Refresh Target](#Refresh_Target)
  - [View Target Table Metrics](#View_Target_Table_Metrics)

**NOTE**: A user can also [Copy a Target](Copy_a_Target_Collect).

**NOTE**: If using DBMoto, [Avoid Timeouts When Building a DBMoto®
Target
Connection](Avoid_Timeouts_When_Building_a_DBMoto_Target_Connection).

## <span id="Register_Targets"></span>Register Targets

Target connections must be SQL Server and located on the same server as
the DSP.

To register a target:

1.  Click **Targets** in the *Navigation* pane.

2.  Click **Add.**
    
    [View the field descriptions for the Targets
    page](../Page_Desc/Targets_H_Collect)

3.  Select a database from the **TARGET** list box.
    
    **NOTE:** The Target must be a valid Data Source.

4.  Click **Save**.

5.  Click **Vertical View** to further configure the Target.

6.  Click **Edit**.
    
    [View the field descriptions for the Targets page's Vertical
    View](../Page_Desc/Targets_H_Collect)

7.  Update the **Collation Type** list box if the default value is not
    applicable.
    
    **NOTE:** The **Collation Type** controls the language option for
    text data in the database. Values are:
    
      - **General Latin Case-insensitive –** collation uses Latin
        characters and is case-insensitive
      - **General Latin Case-sensitive –** collation uses Latin
        characters and is case-sensitive

8.  Update the **Refresh Indices Option** list box if the default value
    is not applicable.
    
    **NOTE:** The **Refresh Indices Option** controls the option to
    build indices or the key of registered tables. Select an option to
    increase the download and network performance. Values are:
    
      - Build Indices and Primary Keys
      - Build Indices only
      - Do Not Build Indices and Primary Keys

9.  Enter additional information about the target in the **Description**
    field; for example, DBA or business contact information, or when the
    target can be deleted from server.

10. Select an ID from the **Data Services ID** list box to assign the
    target to a Data Services implementation, if a Data Services
    instance is used for the creation and execution of packages.
    
    **NOTE:** If using Data Services, set the **Data Services Connection
    Type** at the Target-Source level. Refer to [Configure Source for
    SAP Data
    Services](Register_and_Use_Sources#Configure_Source_for_SAP_Data_Services)
    section for detailed information.
    
    **NOTE:** Consider creating and registering an additional repository
    for separate Target Sources to minimize the chance of overloading
    the communication between Collect and Data Services.

11. Click **Save**.

Continue with Test Target Connection.

## <span id="Test_Target_Connection"></span>Test Target Connection

Test the Data Source connection to verify the database User ID and
Password login credentials are connected to the source or target
databases.

**NOTE:** The Test Connection feature does not test the validity of SAP
login credentials or the DSN connection options.

To test the target database connection:

1.  Click **Targets** in *Navigation* pane.

2.  Select the Target.  

3.  Click **Test Connection** on Page toolbar to test connectivity to
    the target database; a confirmation message displays.

4.  Click **Ok**.

5.  Click **Vertical View** icon to review the connection metrics:

<!-- end list -->

  - **Test ConnectionStatus** – Displays status of the last test
    connection.

  - **Test ConnectionOn** – Displays last date time of test connection.

If a customized ODBC connection is used, the connection string variable
is tested to ensure it can access the database. The SAP user ID,
password and RFC DLL process that utilize the DSN must be verified
outside this process. If a target or a source system password changes,
update the password in the connection table and [rebuild all the
packages from the
source](Register_and_Use_Sources#Build_Package_for_Source).

Continue with Assign Target Security.

## <span id="Assign_Target_Security"></span>Assign Target Security

Security for Collect is assigned at the target level. Target security
limits users’ ability to access and refresh targets. For example, a user
assigned to Material Master might not be allowed to access or refresh
Human Resource source and target databases. The user who creates the
target is automatically granted security; additional users must be
granted security to the target.

To assign target security, an Administrator:

1.  Creates a security role.
2.  Assigns users who are to access the target to the security role.
3.  Assigns WebApp groups to the security role, where

Web App ID = Collect

Group ID = PowerUser

1.  Assigns keys to the Collect Targets security role definition where
    the key is the Target name.

When working with targets, continue with Register Sources.

## <span id="Register_Sources"></span>Register Sources

A *source* is a legacy system from where a copy of data is downloaded
and stored in Collect. Data can be pulled from multiple sources to a
single target; therefore, multiple sources can be registered to a
target.

Refer to [Register Sources to
Target](Register_and_Use_Sources#Register_Sources_to_Target) for
detailed information.

Continue with Refresh Target.

## <span id="Refresh_Target"></span>Refresh Target

*Refreshing* a target is the process of pulling all active tables from
all registered source databases into the target database.

To refresh a target:

1.  Click **Targets** in *Navigation* pane.

2.  Select the Target.

3.  Click **Refresh** on Page toolbar; a confirmation message displays.

4.  Click **Ok**.
    
    **NOTE:** The target is refreshed regardless of the blackout time
    period for the schedule. If the download process is caught during a
    running state (caused by a network or a hardware problem), click
    **Reset** on the *Vertical* View.

Continue with View Target Table Metrics.

## <span id="View_Target_Table_Metrics"></span>View Target Table Metrics

View monthly, weekly and daily metrics for the number of tables
downloaded for a Target.

To view Target metrics:

1.  Click **Targets** in *Navigation* pane.
2.  Click **Metrics** for Target.
3.  Click **Metrics** to view monthly, weekly or daily metrics; a graph
    plotting the metrics displays.
