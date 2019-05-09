+++
title = 'Target Sources H'
solution = 'Platform'
+++

# Target Sources H

[Target Sources V (All Tabs](#Target_Sources_V_All_Tabs))

<div class="use">

Use this page to:

  - [Register Sources to
    Target](../Use_Cases/Register_and_Use_Sources#Register_Sources_to_Target)
  - [Configure Source for SAP Data
    Services](../Use_Cases/Register_and_Use_Sources#Configure_Source_for_SAP_Data_Services)
  - [Schedule Source
    Refresh](../Use_Cases/Refresh_Overview#Schedule_Source_Refresh)
  - [Create
    DBMoto<span style="font-size: 11.0pt;line-height: 107%;font-family: Calibri, sans-serif;mso-ascii-theme-font: minor-latin;mso-fareast-font-family: Calibri;mso-fareast-theme-font: minor-latin;mso-hansi-theme-font: minor-latin;mso-bidi-font-family: &#39;Times New Roman&#39;;mso-bidi-theme-font: minor-bidi;mso-ansi-language: EN-US;mso-fareast-language: EN-US;mso-bidi-language: AR-SA;">®</span>
    Source Connections](../Config/Create_DBMoto_Source_Connections)
  - [Download sdb Tables in
    Collect](../../../Migration/Map/Use_Cases/Download_Tables_Map)
  - [Download dgSAP Tables in
    Collect](../../../Migration/Map/Use_Cases/Download_Tables_Map)

</div>

To access this page:

1.  Click <span style="font-weight: bold;">Collect \> Targets</span> in
    the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Test Connection</p></td>
<td><p>Click to test the connectivity to the data source, which verifies the database User ID and Password login is connected to source database. This process does not test the validity of the SAP login credentials or DSN connection.</p></td>
</tr>
<tr class="odd">
<td><p>Build And Refresh</p></td>
<td><p>Click to build the package and download the table from the source. If the package name already exists for the table record, the table is refreshed (i.e., data is downloaded from the source database). If the package name does not exist, a package is immediately scheduled to be built and the table is refreshed. The Refresh icon is disabled for DBMotoMirror package type because the refresh is run by DBMoto® instead of Collect.</p>
<p><strong>NOTE</strong>: If the data in the target source has been purged manually, or the retention expiration date for that object has passed, it cannot be refreshed and this icon is inactive. Refer to <a href="../Use_Cases/Support_Regulatory_Compliance#Purge_Data">Purge Data</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Import Group Tables</p></td>
<td><p>Click to import system group tables from Common to facilitate adding sources.</p></td>
</tr>
<tr class="odd">
<td><p>Build Package</p></td>
<td><p>Click to build the package that downloads tables from the source.</p>
<p><strong>NOTE</strong>: If the data in the target source has been purged manually, or the retention expiration date for that object has passed, it cannot be refreshed and this icon is inactive. Refer to <a href="../Use_Cases/Support_Regulatory_Compliance#Purge_Data">Purge Data</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Refresh</p></td>
<td><p>Click to download the tables from the source.</p>
<p><strong>NOTE:</strong> If the Target Source uses an IG Universal Connect data source, clicking Refresh executes the Boomi Process.</p>
<p><strong>NOTE:</strong> If the data in the Target Source has been purged manually, or the retention expiration date for that object has passed, it cannot be refreshed and this icon is inactive. Refer to <a href="../Use_Cases/Support_Regulatory_Compliance#Purge_Data">Purge Data</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE</p></td>
<td><p>Displays database where data is refreshed from and stored in the Target. Source is configured when adding a data source in System Administration.</p></td>
</tr>
<tr class="even">
<td><p>CONNECTION TYPE</p></td>
<td><p>Displays valid database connection type from the source to the Target.</p></td>
</tr>
<tr class="odd">
<td><p>SYSTEM TYPE ID</p></td>
<td><p>Displays name of the System Type if importing group tables from a System Type delivered in Common.</p>
<p><strong>NOTE:</strong> Click the + icon to open the System Types page in Common in a new tab to add a System Type, if needed.</p></td>
</tr>
<tr class="even">
<td><p>SCHEMA OWNER</p></td>
<td><p>Displays the schema of the source database that contains the tables. The SCHEMA OWNER doesn’t have to match database user ID. Default value is <strong>dbo</strong></p></td>
</tr>
<tr class="odd">
<td><p>ACTIVE</p></td>
<td><p>If checked, the source is active. Only tables from active sources are downloaded during the refresh process. The default value is Active.</p></td>
</tr>
<tr class="even">
<td><p>Tables</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Tables_H">Tables</a></span> page to add, edit and delete tables for a source.</p></td>
</tr>
<tr class="odd">
<td><p>Schedule Groups</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Target_Source_Group">Target Source Group</a></span> page to build packages, refresh or filter on tables in a group.</p></td>
</tr>
<tr class="even">
<td><p>Metrics</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Target_Source_Metric_Charts">Target Source Metric Charts</a></span> page to view monthly, weekly and daily download results for target/source combination.       </p></td>
</tr>
</tbody>
</table>

## <span id="Target_Sources_V_All_Tabs"></span>Target Sources V (All Tabs)

[Target Sources H](Target_Sources_H_Collect)

<div class="use">

Use this page to:

  - [Register Sources to
    Target](../Use_Cases/Register_and_Use_Sources#Register_Sources_to_Target)
  - [Configure Source for SAP Data
    Services](../Use_Cases/Register_and_Use_Sources#Configure_Source_for_SAP_Data_Services)
  - [Schedule Source
    Refresh](../Use_Cases/Refresh_Overview#Schedule_Source_Refresh)
  - [Create DBMoto™ Source
    Connections](../Config/Create_DBMoto_Source_Connections)
  - [Download sdb Tables in
    Collect](../../../Migration/Map/Use_Cases/Download_Tables_Map)
  - [Download dgSAP Tables in
    Collect](../../../Migration/Map/Use_Cases/Download_Tables_Map)

</div>

This page contains the following tabs:

  - [General tab](#General_Tab)
  - [Advanced Settings tab](#Advanced_Settings_Tab)
  - [Sap Settings tab](#Sap_Settings_Tab)
  - [Action tab](#Action_Tab)
  - [Data Protection tab](#Data_Protection)

## <span id="General_Tab"></span>General tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Build Package</p></td>
<td><p>Click to build a package that downloads tables from the source.</p>
<p><strong>NOTE:</strong> If the data in the Target Source has been purged manually, or the retention expiration date for that object has passed, it cannot be refreshed and this icon is inactive. Refer to <a href="../Use_Cases/Support_Regulatory_Compliance#Purge_Data">Purge Data</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Refresh</p></td>
<td><p>Click to download the tables from the source.</p>
<p><strong>NOTE:</strong> If the Target Source uses an IG Universal Connect data source, clicking Refresh executes the Boomi Process.</p>
<p><strong>NOTE</strong>: If the data in the target source has been purged manually, or the retention expiration date for that object has passed, it cannot be refreshed and this icon is inactive. Refer to <a href="../Use_Cases/Support_Regulatory_Compliance#Purge_Data">Purge Data</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Source</p></td>
<td><p>Displays database where data is refreshed from and stored in the target.</p></td>
</tr>
<tr class="odd">
<td><p>Connection Type</p></td>
<td><p>Displays valid database connection type from the source to the target. Connection Types are configured under Configuration &gt; Connection Types &gt; Sources. Default value is <strong>SQLSERVER</strong>.</p></td>
</tr>
<tr class="even">
<td><p>Schema Owner</p></td>
<td><p>Displays the schema of the source database that contains the tables. The Schema Owner doesn’t have to match database user ID. Default value is dbo.</p></td>
</tr>
<tr class="odd">
<td><p>Description</p></td>
<td><p>Displays additional information about source, for example, DBA or business contact information.</p></td>
</tr>
<tr class="even">
<td><p>System Type ID</p></td>
<td><p>Displays name of the System Type if importing group tables from a System Type delivered with Common.</p>
<p><strong>NOTE:</strong> Click the + icon to open the System Types page in Common in a new tab to add a System Type, if needed.</p></td>
</tr>
<tr class="odd">
<td><p>Test Connection Status</p></td>
<td><p>Displays results from the most recent test connection, either from the Service page or when the Test Connection icon was clicked.</p></td>
</tr>
<tr class="even">
<td><p>Test Connection On</p></td>
<td><p>Displays date and time of the most recent test connection.</p></td>
</tr>
<tr class="odd">
<td><p>Refresh Started On</p></td>
<td><p>Displays date and time when the manual refresh started.</p></td>
</tr>
<tr class="even">
<td><p>Refresh Completed On</p></td>
<td><p>Displays date and time when the manual refresh completed.</p></td>
</tr>
</tbody>
</table>

## <span id="Advanced_Settings_Tab"></span>Advanced Settings tab

Field

Description

Rename Table Template

Displays table name of the renamed table in the target database. At run
time, “\<TableName\>” is replaced by the processing table name.

Schedule ID

Displays schedule for when target tables are refreshed with source data.
Options are controlled in Common \> Configuration \> Schedules. Default
value is **Do Not Download any tables**.

Download Keys Indexes

If checked, primary key indices are refreshed from non-SAP sources.

It is checked by default.

Delete Target Table On Build

If checked, all previously refreshed tables are deleted and tables (and
primary keys and indices) are rebuilt each time the package is built.
This setting ensures the most recent table schema is downloaded. Default
value is Disabled.

**NOTE:** It is recommended that the Delete Target Table On Build check
box be unchecked if the package type to download table data is set to
SAP Data Services. In this case, if the check box is checked,
dspCompose™ WILL delete every record in the target table during the
Final Finish process (during which data posted in the target ERP system
by the request is downloaded to tables).

Data Services

Do Not Delete Data

If checked, the data is **NOT** deleted before it is refreshed when the
Refresh icon is clicked on the *Horizontal* View. Data Services must be
set to CDC (Change Data Capture) for each table in the source when using
DBMoto or Data Services.

**NOTE**: This check box displays if a Data Services ID is selected.

Data Services ID

Displays the repository used for the target source.

If this field is blank, the repository set at the target level is used
for the target source.

Setting a repository for a target source is useful if there are a large
number of jobs to run.

This repository is used for the target source Data Services repository,
where Data Services jobs for the source system can be registered and run
against.

**NOTE:** Set a repository for each target or target source. There is a
limit on the number of Collect jobs that can be created in a single Data
Services repository. Consider creating and registering an additional
repository for separate target sources to minimize the chance of
overloading the communication between Collect and Data Services.

Data Services Connection Type

Displays database connection type when using Data Services.

Connection Settings

Click to open the <span style="font-style: italic;">[Target Sources -
DataServices Connection](Target%20Summary)</span> page to edit the
database connection settings for Data Services.

Boomi

Boomi Data Source

Displays the name of the IG Universal Connect data source registered in
Common used when the Boomi Processes are executed.

**NOTE:** This field only displays if the source is an IG Universal
Connect data source.

Boomi Atom Override

Displays the name of the atom, the default execution environment where
the Boomi Process runs.

If this field is blank, the Process executes against the default atom
registered with the IG Universal Connect data source.

**NOTE:** This field allows the user to run the Target Source refresh
against a registered atom other than the one assigned to the default
data source. Use this feature for testing purposes if there are multiple
atoms set up on different DSP® server environments and the tests should
be run against the different environments registered under the single
tenant.

**NOTE:** This field only displays if the source is an IG Universal
Connect data source.

## <span id="Sap_Settings_Tab"></span>Sap Settings tab

Field

Description

SAP User ID

Displays user ID to log into SAP. Used for RFC and SAP Text data
downloads.

SAP Password

Displays encrypted password to log into SAP. Used for RFC and SAP Text
data downloads.

Client

Displays the name of the client within the SAP instance. Used for RFC
and SAP Text data downloads.

**NOTE:** The information in this field is used to filter the data
downloaded from the source. The filter runs against the MANDT column.

All Clients

If checked, data is downloaded for all clients in the SAP instance. Used
for RFC and SAP Text data downloads. Default value is unchecked.

Remove Client From Key

If checked, builds primary keys without the client field (usually
MANDT). This feature can only be used if only 1 client is downloaded
(i.e., All Clients is unchecked).  Used for RFC and SAP Text data
downloads. Default value is unchecked.

Instance

Displays SAP instance name used for the source refresh.

Language

Displays default language of the SAP instance.

SAP System Number

Displays system number used to log into SAP so Collect can refresh Pool
Table data.

SAP Server Host

Displays server host used to log into SAP so Collect can download Pool
Table data from the source.

Test Sap Connection

Click to test connection to SAP. This process doesn't test the validity
of the SAP User ID or Password, or verifies the SAP User ID has access
to SAP tables; only verifies SAP User ID has access to SAP.

Sap Optional

Rfc Name Space Option

Displays option for RFC namespace, as in, the type of SAP transport that
is used. The default option is configured in Common \> Collect
Parameters.

Values are:  NAMESPACE, NONNAMESPACE

BackOffice Associates® owns the namespace /BOA. The NonNamespace
transports begin with ZBOA. Check with BASIS team to find out if you are
running NAMESPACE or NONNAMESPACE.

SAP Msg Server Host

Displays the server host name if SAP Load Balancing is used to download
SAP table from the source via RFC. Refer to SAP documentation for
details about Load Balancing.

SAP Logon Group

Displays the logon group name if SAP Load Balancing is used to download
SAP table from the source via RFC. Refer to SAP documentation for
details about Load Balancing.

###  

## <span id="Action_Tab"></span>Action tab

 

Field

Description

Fetch Tables

Click to download tables from the source into a new System Type group
with the same name as the source. This process is helpful for source
database systems where many tables must be created and downloaded. A
System Type group is added for each schema with the naming convention of
\<source\>\_\<schemaowner\>. Refer to [Create System Type Groups from
the Fetch
Process](../Use_Cases/Create_Groups_from_the_Fetch_Process).

Reset

Click to reset the status of the source and all its tables. This process
activates the Refresh icon and triggers the batch job schedule to
calculate new run dates for the next scheduled refresh. Reset doesn’t
impact processes currently running. Reset target if download process
backs up due to network problems.

Build Groups

Click to build System Type groups from existing source tables after the
source is configured. A System Type group is created with the naming
convention \<Target\>\_\<Source\> and the schema owner is defaulted to
dbo for the group. Refer to [Create System Type Groups from Source
Tables](../Use_Cases/Create_a_System_Type_Group_from_Source_Tables).

Fetch Table Options

Activate Fetched Tables

Click to activate tables in the fetch table process.

 

 

## <span id="Data_Protection"></span>Data Protection

<div class="use">

Use this tab to:

  - [Configure Data
    Protection](../Use_Cases/Support_Regulatory_Compliance#Configure_Data_Protection)
  - [Update the Retention Expiration
    Date](../Use_Cases/Support_Regulatory_Compliance#Update_the_Retention_Expiration_Date)
  - [Purge
    Data](../Use_Cases/Support_Regulatory_Compliance#Purge_Data)

</div>

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Data Controller</p></td>
<td><p>Displays the user responsible for the processing of personal data in the target source.</p>
<p>Any user or group who is assigned the Data Controller role must have a user account in the DSP. Data Controller must have access to the target based on their assigned security role and security key.</p>
<p><strong>NOTE</strong>: The Collect Administrator must check the WORK FLOW SUMMARY check box for the target and Data Controller on the <em><a href="Workflow_Summary_User_Settings">Workflow Summary User Settings</a></em> page. The Data Controller is added to this page automatically. If the check box is not checked, the Data Controller will not receive a warning email that data is going to be purged.</p></td>
</tr>
<tr class="odd">
<td><p>Data Classification</p></td>
<td><p>Displays the nature of the data in the target source, identifying whether it contains personal data and so must be purged for regulatory compliance.</p>
<p>Options included with the DSP are:</p>
<ul>
<li><strong>Personal</strong> — This object contains data that must be purged by a certain date. The Retention Expiration Date field must be completed for this object (for example, Customer Addresses, Employee Records, Business Partner Tax IDs).</li>
<li><strong>Public</strong> —This object contains data that does not need to be purged (for example, Units of Measure, Material Descriptions, Country Codes).</li>
<li><strong>Restricted</strong> — This data does not need to be purged, but is marked as restricted access (for example, Company Chart of Accounts, Recipes, Work Orders).</li>
</ul>
<p><strong>NOTE:</strong> These options are delivered with the DSP and cannot be updated; however, a Common Administrator can create custom classifications on the Data Classification page in Common. Refer to <a href="../../Common/Use_Cases/Add%20Custom%20Data%20Classifications%20and%20Information%20Types">Add Custom Data Classifications and Information Types</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Retention Expiration Date</p></td>
<td><p>Displays the date when the data in the Target Sources and tables will be automatically purged when a Service page runs.</p>
<p>A Collect Administrator must enter a date for a target source with a data classification of Personal or for any custom classification with the Retention Period Warning feature enabled.</p>
<p>A different retention expiration date can be set at the target and table level.</p>
<p>If no date is set for the object, the data is not purged.</p>
<p><strong>NOTE:</strong> Updates to this field are audited. An e-signature is required.</p>
<p><strong>NOTE:</strong> Once this data has passed, the Refresh and Build and Refresh icons on the <a href="Targets_H_Collect">Targets</a><em>,</em> <a href="Tables_H">Tables</a> and this page are inactive. The table can no longer be refreshed either manually or automatically.</p></td>
</tr>
<tr class="odd">
<td><p>Data Collection Reason</p></td>
<td><p>Displays reason for extracting the data. Any time the Target Source is processed, the data should only be used for the reason identified in this field.</p></td>
</tr>
<tr class="even">
<td><p>Purge Data</p></td>
<td><p>Click to manually delete all data in all tables (including check tables) at the target source and table levels.</p>
<p><strong>NOTE:</strong> Data is automatically purged on the Retention Expiration Date when a Service page runs once daily.</p>
<p><strong>NOTE:</strong> After data is purged, the table(s) cannot be downloaded again for the target, and the Collect refresh will not pull data into the table. The Refresh and Build and Refresh icons on the Targets, Target Sources, and Tables pages are inactive.</p></td>
</tr>
</tbody>
</table>
